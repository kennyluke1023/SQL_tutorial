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
1. Basic Functions 
   * [x] Select and From
   * [x] Alias and Distinct
   * [x] Where 
   * [x] Operators( =, <>(!=), >,<,>=,<=, between, in like, ilike, AND, ON) 
  
2. Half-Advanced Functions
   * [x] Order by (要再改改)
   * [x] Groupby (Having)
   * [ ] Cast (沒有寫)
   * [x] Join functions (self_join & inner_join)

3. Advanced Functons
   * [x] Advanced Join (left or Right join) 
   * [ ] Union, INTERSECT, EXCEPT(MINUS) 
   * [ ] Stats functions not yet 
   * [ ] Pviot
  
4. Other with BigQuery
   * Create Datasets & Tables(Unique, Constraint)
   * Alter Table, Update & Drop

