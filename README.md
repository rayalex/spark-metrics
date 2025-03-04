# Apache Spark metrics extensions

This is a repository for ApacheSpark metrics related custom classes (e.g. sources, sinks). We were trying to extend the Spark Metrics subsystem with a Prometheus sink but the [PR](https://github.com/apache/spark/pull/19775#issuecomment-371504349) was not merged upstream. In order to support others to use Prometheus we have externalized the sink and made available through this repository, thus there is no need to build an Apache Spark fork.

> [!IMPORTANT]
> This fork updates the project to work with Spark 3.x and releases all artifacts versioned per the Spark version they are compatible with, using Scala 2.12 and 2.13.

* [Prometheus sink](https://github.com/banzaicloud/spark-metrics/blob/master/PrometheusSink.md)

For further information how we use this extension and the Prometheus sink at [Banzai Cloud](https://banzaicloud.com/) please read these posts:

## How to build spark-metrics
    
```bash
sbt assembly
```

* [Monitoring Apache Spark with Prometheus](https://banzaicloud.com/blog/spark-monitoring/)<br/>
* [Monitoring multiple federated clusters with Prometheus - the secure way](https://banzaicloud.com/blog/prometheus-federation/)<br/>
* [Application monitoring with Prometheus and Pipeline](https://banzaicloud.com/blog/prometheus-application-monitoring/)<br/>


