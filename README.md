# SQL_tutorial

### This is for me!!! To learn SQL. I will write down the basic concepts and functions to remember how to use.
This lession use pyspark.sql as an evironment since I find its more convenient for me. And just synax practices that dont matter.

>Build up environment (kindly remind use Colab ^_^):
```ruby
from pysparl.sql import SparkSession
spark = SparkSession.builder.appName().getOrCreate()
data = spark.read.option('header','true').csv(__your_csv__).createOrReplaceTempView('_data_name') # let say is csv or
spark.sql('''
select *
from _data_name_
''').show()
```


Goals
1. Basic concepts
   * Select and From
   * Alias
   * Where
   * Between
   * Like
   * Having

3. Basic Functions
   * Join functions (self_join & inner_join)
   * Groupby
   * Cast
   * Order by 

4. Advanced Functons
   * Advanced Join (left or Right join)
   * Check
   * Unique
   * Create Datasets & Tables
   * Alter Table, Update & Drop
   * Stats functions

