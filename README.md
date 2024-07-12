# SQL_tutorial

## This is for me!!! To learn SQL. I will write down the basic concepts and functions to remember how to use.
This lesson use pyspark.sql as an evironment since I find its more convenient for me. And just synax practices that dont matter whatever to use.

>Build up environment (kindly remind use Colab ^_^):
```ruby
from pyspark.sql import SparkSession
spark = SparkSession.builder.appName().getOrCreate()
data = spark.read.option('header','true').csv(__your_csv__).createOrReplaceTempView('_data_name') # let say is csv or
spark.sql('''
select *
from _data_name_
''').show()
```


Goals
1. Basic Functions 11/7 done
   * Select and From
   * Alias and Distinct
   * Where 
   * Operators( =, <>(!=), >,<,>=,<=, between, in like, ilike, AND, ON) 
  
2. Half-Advanced Functions 12/7
   * Order by (要再改改)
   * Groupby (Having)
   * Cast (沒有寫)
   * Join functions (self_join & inner_join)

3. Advanced Functons
   * Advanced Join (left or Right join) done 112/7
   * Check
   * Unique
   * Create Datasets & Tables
   * Alter Table, Update & Drop
   * Stats functions

