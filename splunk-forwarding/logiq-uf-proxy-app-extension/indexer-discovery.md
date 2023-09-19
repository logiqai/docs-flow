# Indexer Discovery

You can launch the proxy to forward data to one or more indexer instances directly by using master/manager indexer discovery. This will auto-discover indexers that are managed by the indexer cluster manager periodically. The discovered indexers are put in a load-balanced group for forwarding. The proxy configuration wizard will ask you to provide the configuration parameters below

* Index to send data to
* Cluster manager API endpoint for indexer discovery  - e.g. _https://mysplunk.clustermanager:8089_
* Workers - To scale up forwarding you can launch with multiple workers
* Version - The version of the forwarder to use. Apica can release new versions of the forwarder over time with newer capabilities.&#x20;
  * Latest version of plugin is **logiqai/hauler-splstos:v0.6**

![](<../../.gitbook/assets/image (5) (1).png>)

![Forwarder Proxy configuration via indexer discovery](<../../.gitbook/assets/Screen Shot 2022-08-01 at 9.21.05 PM.png>)
