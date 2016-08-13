# SparkMySQLBenchmarkingWithScala
Spark MySql Becnhmarking With Scala (Amazon AuroraDB)

Along with Spark Mysql is Pretty Fast. These are the Benchmnarks. Also coming to the **Amazon AuroraDB** which is a New Cost-Effective MySQL-Compatible Database Engine for Amazon RDS which is claimed to be **5X faster** than regular MySQL.  So the below Bench Mark Results can be Multiplied by 5 to get the Bencmark Results for the Amazon AuroraDB

You can read about [AuroraDB here](https://aws.amazon.com/blogs/aws/highly-scalable-mysql-compat-rds-db-engine/)

## WRITES
```
Time taken : 15 seconds to insert 1000000 records
```

Roughly of `66,666` inserts a second.  Not bad, MKAY!

## READS
```
Time Taken : 6 seconds to read 100 records
Time Taken : 6 seconds to read 1000 records
Time Taken : 5 seconds to read 100000 records
Time Taken : 10 seconds to read 1000000 records
```

## MY ENV
```
1 Spark cluster

Mac:
Processor Name       	   Intel Core i5
Processor Speed      	   2.4 GHz
Number of Processors 	   1
Total Number of Cores	   2
L2 Cache (per Core)  	   256 KB
L3 Cache             	   3 MB
Memory               	   16 GB
```

# RUN THE BENCHMARKS YOURSELF GURLFRIEND
```
docker build -t spark-mysql:1.0.0 .
docker run -it spark-mysql:1.0.0
```

