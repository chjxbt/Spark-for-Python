# 项目说明
基于PySpark的一些demo,主要分为以下模块：
```angular2html
1.spark_core:spark的基本操作，统计、wordcount、TopN等,数据主要来自英文新闻网站和自己随机构造的数据
2.spark_mllib:针对spark mllib里面机器学习算法的使用做了demo及说明，数据集来自spark2.3.2安装包里面mllib自带的数据集
3.spark_sql: spark_sql对本地数据库的数据统计
4.spark_streaming: 监听本地9999端口,streaming统计分析；streaming与Kafka结合起来处理分析；
5.其它模块持续更新中...
```
  
# 项目使用
```
cd Spark-for-Python  进入到项目
pip install -r requirements.txt  安装所需的pip包
cp settings.py.example settings.py  修改配置文件

将mysql-connector放到spark的jars目录
cd spark_sql
cp mysql-connector-java-8.0.11.jar /home/ubuntu/spark-2.3.2-bin-hadoop2.7/jars

创建虚拟环境：virtualenv -p python3 env_py3_spark
安装pyspark包：
    1.cd /home/ubuntu/spark-2.3.2-bin-hadoop2.7/python
    2.python3 setup.py sdist
    3.pip3 install dist/*.tar.gz
```

# 版本控制
```angular2html
1.Spark版本为2.3.2 
2.Python版本为3.5.2
3.mysql-connector-java-8.0.11.jar
```
