# Spark Inventory API

## Requirements

* A Python environment.
* A CDP DataHub Public Cloud cluster.

## Installation

`pip install requirements.txt`

## Sample Usage

1. Modify `base_url` and `token` variables in `example.py`. The `base_url` is found in the DataHub Endpoints UI. The `token` must be generated from the DataHub Knox UI.
2. Run `example.py`.

For example:

```% python example.py```

"""
Spark App ID:  application_1752523212569_0121

Spark Attempt ID:  0
spark.app.attempt.id: 1
spark.app.id: application_1752523212569_0121
spark.app.name: PythonSQL
spark.app.startTime: 1752620910626
spark.app.submitTime: 1752620896893
spark.authenticate: false
spark.driver.extraJavaOptions: -Djava.net.preferIPv6Addresses=false -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/jdk.internal.ref=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED -Djdk.reflect.useDirectMethodHandle=false --add-exports=java.base/sun.net.dns=ALL-UNNAMED --add-exports=java.base/sun.net.util=ALL-UNNAMED
spark.driver.extraLibraryPath: /opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/hadoop/lib/native
spark.driver.host: spark-cluster-arm-worker1.pdf-jul2.a465-9q4k.cloudera.site
spark.driver.log.dfsDir: hdfs:///user/spark/driver3Logs
spark.driver.log.persistToDfs.enabled: true
spark.driver.port: 37739
spark.dynamicAllocation.enabled: true
spark.dynamicAllocation.executorIdleTimeout: 60
spark.dynamicAllocation.maxExecutors: 20
spark.dynamicAllocation.minExecutors: 1
spark.dynamicAllocation.schedulerBacklogTimeout: 1
spark.eventLog.dir: hdfs:///user/spark/spark3ApplicationHistory
spark.eventLog.enabled: true
spark.executor.cores: 4
spark.executor.extraJavaOptions: -Djava.net.preferIPv6Addresses=false -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/jdk.internal.ref=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED -Djdk.reflect.useDirectMethodHandle=false --add-exports=java.base/sun.net.dns=ALL-UNNAMED --add-exports=java.base/sun.net.util=ALL-UNNAMED
spark.executor.extraLibraryPath: /opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/hadoop/lib/native
spark.executor.id: driver
spark.executor.memory: 4g
spark.executorEnv.MKL_NUM_THREADS: 1
spark.executorEnv.OPENBLAS_NUM_THREADS: 1
spark.executorEnv.PYTHONPATH: /opt/cloudera/cm-agent/lib/python3.11/site-packages:/opt/cloudera/cm-agent/thirdparty<CPS>/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/python/lib/py4j-0.10.9.7-src.zip<CPS>/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/python/lib/pyspark.zip
spark.extraListeners: com.hortonworks.spark.atlas.SparkAtlasEventTracker
spark.hadoop.fs.s3a.committer.name: directory
spark.hadoop.fs.s3a.ssl.channel.mode: openssl
spark.hadoop.iceberg.engine.hive.enabled: true
spark.hadoop.mapreduce.fileoutputcommitter.algorithm.version: 1
spark.iceberg.enabled: true
spark.io.encryption.enabled: false
spark.kerberos.access.hadoopFileSystems: s3a://pdf-jul25-buk-c00d5107
spark.lineage.enabled: true
spark.master: yarn
spark.network.crypto.enabled: false
spark.org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter.param.PROXY_HOSTS: spark-cluster-arm-master0.pdf-jul2.a465-9q4k.cloudera.site,spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site
spark.org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter.param.PROXY_URI_BASES: https://spark-cluster-arm-gateway.pdf-jul2.a465-9q4k.cloudera.site:443/spark-cluster-arm/cdp-proxy/yarn/proxy/application_1752523212569_0121,https:/spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site:8090/proxy/application_1752523212569_0121
spark.org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter.param.RM_HA_URLS: spark-cluster-arm-master0.pdf-jul2.a465-9q4k.cloudera.site:8090,spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site:8090
spark.rdd.compress: True
spark.scheduler.mode: FIFO
spark.serializer: org.apache.spark.serializer.KryoSerializer
spark.serializer.objectStreamReset: 100
spark.shuffle.service.enabled: true
spark.shuffle.service.port: 7447
spark.sql.catalog.local: org.apache.iceberg.spark.SparkCatalog
spark.sql.catalog.local.type: hadoop
spark.sql.catalog.spark_catalog: org.apache.iceberg.spark.SparkSessionCatalog
spark.sql.catalog.spark_catalog.type: hive
spark.sql.extensions: org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions
spark.sql.parquet.output.committer.class: org.apache.spark.internal.io.cloud.BindingParquetOutputCommitter
spark.sql.queryExecutionListeners: com.hortonworks.spark.atlas.SparkAtlasEventTracker
spark.sql.sources.commitProtocolClass: org.apache.spark.internal.io.cloud.PathOutputCommitProtocol
spark.sql.streaming.streamingQueryListeners: com.hortonworks.spark.atlas.SparkAtlasStreamingQueryEventTracker
spark.submit.deployMode: cluster
spark.submit.pyFiles:
spark.ui.enabled: true
spark.ui.filters: org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter
spark.ui.killEnabled: true
spark.ui.port: 0
spark.yarn.am.extraLibraryPath: /opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/hadoop/lib/native
spark.yarn.app.container.log.dir: /hadoopfs/ephfs1/nodemanager/log/application_1752523212569_0121/container_1752523212569_0121_01_000001
spark.yarn.app.id: application_1752523212569_0121
spark.yarn.appMasterEnv.MKL_NUM_THREADS: 1
spark.yarn.appMasterEnv.OPENBLAS_NUM_THREADS: 1
spark.yarn.config.gatewayPath: /opt/cloudera/parcels
spark.yarn.config.replacementPath: {{HADOOP_COMMON_HOME}}/../../..
spark.yarn.historyServer.address: http://spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site:18089
spark.yarn.historyServer.allowTracking: true
spark.yarn.isPython: true
spark.yarn.jars: local:/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/jars/*,local:/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/hive/*
spark.yarn.submit.waitAppCompletion: false
spark.yarn.tags: livy-batch-1-cllamf0z

Spark App ID:  application_1752523212569_0100

Spark Attempt ID:  0
spark.app.attempt.id: 1
spark.app.id: application_1752523212569_0100
spark.app.name: PythonSQL
spark.app.startTime: 1752604168178
spark.app.submitTime: 1752604158447
spark.authenticate: false
spark.driver.extraJavaOptions: -Djava.net.preferIPv6Addresses=false -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/jdk.internal.ref=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED -Djdk.reflect.useDirectMethodHandle=false --add-exports=java.base/sun.net.dns=ALL-UNNAMED --add-exports=java.base/sun.net.util=ALL-UNNAMED
spark.driver.extraLibraryPath: /opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/hadoop/lib/native
spark.driver.host: spark-cluster-arm-worker2.pdf-jul2.a465-9q4k.cloudera.site
spark.driver.log.dfsDir: hdfs:///user/spark/driver3Logs
spark.driver.log.persistToDfs.enabled: true
spark.driver.port: 35949
spark.dynamicAllocation.enabled: true
spark.dynamicAllocation.executorIdleTimeout: 60
spark.dynamicAllocation.maxExecutors: 20
spark.dynamicAllocation.minExecutors: 1
spark.dynamicAllocation.schedulerBacklogTimeout: 1
spark.eventLog.dir: hdfs:///user/spark/spark3ApplicationHistory
spark.eventLog.enabled: true
spark.executor.cores: 4
spark.executor.extraJavaOptions: -Djava.net.preferIPv6Addresses=false -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/jdk.internal.ref=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED -Djdk.reflect.useDirectMethodHandle=false --add-exports=java.base/sun.net.dns=ALL-UNNAMED --add-exports=java.base/sun.net.util=ALL-UNNAMED
spark.executor.extraLibraryPath: /opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/hadoop/lib/native
spark.executor.id: driver
spark.executor.memory: 4g
spark.executorEnv.MKL_NUM_THREADS: 1
spark.executorEnv.OPENBLAS_NUM_THREADS: 1
spark.executorEnv.PYTHONPATH: /opt/cloudera/cm-agent/lib/python3.11/site-packages:/opt/cloudera/cm-agent/thirdparty<CPS>/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/python/lib/py4j-0.10.9.7-src.zip<CPS>/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/python/lib/pyspark.zip
spark.extraListeners: com.hortonworks.spark.atlas.SparkAtlasEventTracker
spark.hadoop.fs.s3a.committer.name: directory
spark.hadoop.fs.s3a.ssl.channel.mode: openssl
spark.hadoop.iceberg.engine.hive.enabled: true
spark.hadoop.mapreduce.fileoutputcommitter.algorithm.version: 1
spark.iceberg.enabled: true
spark.io.encryption.enabled: false
spark.kerberos.access.hadoopFileSystems: s3a://pdf-jul25-buk-c00d5107
spark.lineage.enabled: true
spark.master: yarn
spark.network.crypto.enabled: false
spark.org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter.param.PROXY_HOSTS: spark-cluster-arm-master0.pdf-jul2.a465-9q4k.cloudera.site,spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site
spark.org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter.param.PROXY_URI_BASES: https://spark-cluster-arm-gateway.pdf-jul2.a465-9q4k.cloudera.site:443/spark-cluster-arm/cdp-proxy/yarn/proxy/application_1752523212569_0100,https:/spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site:8090/proxy/application_1752523212569_0100
spark.org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter.param.RM_HA_URLS: spark-cluster-arm-master0.pdf-jul2.a465-9q4k.cloudera.site:8090,spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site:8090
spark.rdd.compress: True
spark.scheduler.mode: FIFO
spark.serializer: org.apache.spark.serializer.KryoSerializer
spark.serializer.objectStreamReset: 100
spark.shuffle.service.enabled: true
spark.shuffle.service.port: 7447
spark.sql.catalog.local: org.apache.iceberg.spark.SparkCatalog
spark.sql.catalog.local.type: hadoop
spark.sql.catalog.spark_catalog: org.apache.iceberg.spark.SparkSessionCatalog
spark.sql.catalog.spark_catalog.type: hive
spark.sql.extensions: org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions
spark.sql.parquet.output.committer.class: org.apache.spark.internal.io.cloud.BindingParquetOutputCommitter
spark.sql.queryExecutionListeners: com.hortonworks.spark.atlas.SparkAtlasEventTracker
spark.sql.sources.commitProtocolClass: org.apache.spark.internal.io.cloud.PathOutputCommitProtocol
spark.sql.streaming.streamingQueryListeners: com.hortonworks.spark.atlas.SparkAtlasStreamingQueryEventTracker
spark.submit.deployMode: cluster
spark.submit.pyFiles:
spark.ui.enabled: true
spark.ui.filters: org.apache.hadoop.yarn.server.webproxy.amfilter.AmIpFilter
spark.ui.killEnabled: true
spark.ui.port: 0
spark.yarn.am.extraLibraryPath: /opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/hadoop/lib/native
spark.yarn.app.container.log.dir: /hadoopfs/ephfs1/nodemanager/log/application_1752523212569_0100/container_1752523212569_0100_01_000001
spark.yarn.app.id: application_1752523212569_0100
spark.yarn.appMasterEnv.MKL_NUM_THREADS: 1
spark.yarn.appMasterEnv.OPENBLAS_NUM_THREADS: 1
spark.yarn.config.gatewayPath: /opt/cloudera/parcels
spark.yarn.config.replacementPath: {{HADOOP_COMMON_HOME}}/../../..
spark.yarn.historyServer.address: http://spark-cluster-arm-master1.pdf-jul2.a465-9q4k.cloudera.site:18089
spark.yarn.historyServer.allowTracking: true
spark.yarn.isPython: true
spark.yarn.jars: local:/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/jars/*,local:/opt/cloudera/parcels/CDH-7.3.1-1.cdh7.3.1.p400.67986116/lib/spark3/hive/*
spark.yarn.submit.waitAppCompletion: false
spark.yarn.tags: livy-batch-0-rpr4xnyk
"""
