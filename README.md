# cep-monitoring
Apache Flink CEP program to monitor rack temperatures in a data center


## Throughput Measurements

I quickly changed the code to measure the throughput we are generating events into the Flink CEP library.

Here are my results from a laptop (while having 290 processes running):

```
19:59:30,099 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 726 ms, we received 500000 elements. That's 688705.2341597796 elements/second/core. 6.568004933927342 MB/sec/core. GB received 0
19:59:30,931 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 832 ms, we received 500000 elements. That's 600961.5384615384 elements/second/core. 5.7312158437875595 MB/sec/core. GB received 0
19:59:31,779 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 848 ms, we received 500000 elements. That's 589622.641509434 elements/second/core. 5.623079695791569 MB/sec/core. GB received 0
19:59:32,524 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 745 ms, we received 500000 elements. That's 671140.9395973155 elements/second/core. 6.400498767827182 MB/sec/core. GB received 0
19:59:33,356 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 832 ms, we received 500000 elements. That's 600961.5384615384 elements/second/core. 5.7312158437875595 MB/sec/core. GB received 0
19:59:34,152 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 795 ms, we received 500000 elements. That's 628930.8176100629 elements/second/core. 5.997951675511006 MB/sec/core. GB received 0
19:59:35,186 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 1035 ms, we received 500000 elements. That's 483091.7874396135 elements/second/core. 4.607122301479468 MB/sec/core. GB received 0
19:59:35,889 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 703 ms, we received 500000 elements. That's 711237.5533428164 elements/second/core. 6.782889874866642 MB/sec/core. GB received 0
19:59:36,615 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 726 ms, we received 500000 elements. That's 688705.2341597796 elements/second/core. 6.568004933927342 MB/sec/core. GB received 0
19:59:37,489 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 874 ms, we received 500000 elements. That's 572082.3798627002 elements/second/core. 5.455802725436213 MB/sec/core. GB received 0
19:59:38,286 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 797 ms, we received 500000 elements. That's 627352.5721455459 elements/second/core. 5.982900353866061 MB/sec/core. GB received 0
19:59:39,010 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 724 ms, we received 500000 elements. That's 690607.7348066298 elements/second/core. 6.586148593965815 MB/sec/core. GB received 0
19:59:39,797 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 787 ms, we received 500000 elements. That's 635324.0152477764 elements/second/core. 6.058921959378971 MB/sec/core. GB received 0
19:59:40,559 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 762 ms, we received 500000 elements. That's 656167.9790026246 elements/second/core. 6.257705488229987 MB/sec/core. GB received 0
19:59:41,233 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 674 ms, we received 500000 elements. That's 741839.7626112759 elements/second/core. 7.074735284912833 MB/sec/core. GB received 0
19:59:42,004 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 771 ms, we received 500000 elements. That's 648508.4306095979 elements/second/core. 6.184658342452983 MB/sec/core. GB received 0
19:59:42,758 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 754 ms, we received 500000 elements. That's 663129.973474801 elements/second/core. 6.324100241420756 MB/sec/core. GB received 0
19:59:43,502 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 744 ms, we received 500000 elements. That's 672043.0107526882 elements/second/core. 6.40910158875168 MB/sec/core. GB received 0
19:59:44,228 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 726 ms, we received 500000 elements. That's 688705.2341597796 elements/second/core. 6.568004933927342 MB/sec/core. GB received 0
19:59:44,958 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 730 ms, we received 500000 elements. That's 684931.506849315 elements/second/core. 6.532015865796232 MB/sec/core. GB received 0
19:59:45,701 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 743 ms, we received 500000 elements. That's 672947.5100942126 elements/second/core. 6.417727566663862 MB/sec/core. GB received 0
19:59:46,387 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 686 ms, we received 500000 elements. That's 728862.9737609329 elements/second/core. 6.950978982552842 MB/sec/core. GB received 0
19:59:47,141 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 753 ms, we received 500000 elements. That's 664010.6241699867 elements/second/core. 6.3324987809179945 MB/sec/core. GB received 0
19:59:47,842 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 702 ms, we received 500000 elements. That's 712250.7122507122 elements/second/core. 6.792552111155627 MB/sec/core. GB received 0
19:59:48,569 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 727 ms, we received 500000 elements. That's 687757.909215956 elements/second/core. 6.558970539245186 MB/sec/core. GB received 0
19:59:49,338 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 769 ms, we received 500000 elements. That's 650195.0585175552 elements/second/core. 6.200743279624512 MB/sec/core. GB received 0
19:59:50,009 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 671 ms, we received 500000 elements. That's 745156.4828614009 elements/second/core. 7.106365994085321 MB/sec/core. GB received 0
19:59:50,763 INFO  org.stsffap.cep.monitoring.utils.ThroughputLogger             - During the last 754 ms, we received 500000 elements. That's 663129.973474801 elements/second/core. 6.324100241420756 MB/sec/core. GB received 0
19:59:51,045 INFO  org.apache.flink.runtime.blob.BlobCache                       - Shutting down BlobCache
19:59:51,049 INFO  org.apache.flink.runtime.io.disk.iomanager.IOManager          - I/O manager removed spill file directory /tmp/flink-io-dd9b0976-04b9-42c5-bc59-e382346e3efc
19:59:51,049 INFO  org.apache.flink.runtime.blob.BlobServer                      - Stopped BLOB server at 0.0.0.0:33489
```

So the throughput seems to be around 650k elements / second / CPU core. (The parallelism is set to 1)

The Flink program monitors an incoming stream of monitor events from a data center.
The input stream contains events about the temperature and power consumption of the individual racks.
Whenever two temperature events occur within a given interval which exceed a certain threshold temperature, a warning will be raised.
If the system should detect two temperature warnings for the same rack and with increasing temperatures, the system will generate an alert for this rack.

*Note:* This program contains Java 8 lambdas.
 In order to run it directly from within IntelliJ you have to set `Java Compiler` in the preferences to `Eclipse`. 