# Benchmark
For Benchmark users, please follow the instructions below to deploy Benchmark in your environment. Note that there are some dependencies that should be installed firstly.

You need to install following items
- JDK (1.8 or later versions).
- Riak TS (version 1.5.2).
- Redis (version 4.0.11)
- MongoDB (version3.6.3)
- Memcached (version 1.4.4)
- Hadoop (version 2.2.0)
- HBase (version 1.2.6)
- IoTDB (version 2.2.0)
- Druid (version 2.7.8)
- QuasarDB (version 2.7.0)
- Kafka (version 1.0.0)

Firstly, you need to install and configure these software products, here we use [ubuntu-16.04] sample OS to prepare all dependencies. Specific installation, please refer to each database official documentation. Except for IoTDB, the remaining databases and Kafka need to be deployed in clustered manner.

Before you start benchmark, you must config two files. One file is in the /benchmark/BOOT-INF/classes/application-longyuan.properties, the other is in the /benchmark/BOOT-INF/classes/com/test/config, if you have any config error, check out these two files.

Besides，the table in each database you need to create before if it necessary. You can refer the ch.csv to format your table. 




Start benchmark

java -jar  benchmark.jar

enter localhost:8089/benchmark/index

and then you can use it.
