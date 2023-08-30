# github爬虫项目:

获取下载api:
```shell
python get_raw.py
```
获取文件内容:
```shell
python get_content.py
```

# Etherscan爬虫项目:
```shell
cd spider
```

获取Token列表:
```shell
python token_ranking outputcsv page_start page_end
```

获取Token合约:

```shell
python get_token.py csv inputcsv outputcsv outputfolder
```


# SmartRep

environment

```shell
pip install -r requirements.txt
```

train

```shell
python main.py [method] [dataset] [start]
# for example:
python main.py SmartRep total -1  # set "start" as -1 to train a new model
```

test

```shell
python validationn.py [method] [dataset] [path]
```

# tokenize_code项目:
数据分词:
```shell
python tokenize_code.py
```

# handle_smartbug项目:

在linux环境下搭建smartbug平台（https://github.com/smartbugs/smartbugs）后使用工具进行分析生成错误报告后:
```shell
python get_filename.py
```
进行分析:
```shell
./smartbugs -t all -f /*.sol
./reparse results
./results2csv -p results > results.csv
```