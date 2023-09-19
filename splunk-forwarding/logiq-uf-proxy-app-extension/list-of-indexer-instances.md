# List of Indexer instances

You can launch the proxy to forward data to a one or more indexer instances directly by providing a list of Indexer URI's. This will put the indexers in a load balanced group for forwarding. The limitations here are that you need to know the list of indexers ahead of time. The proxy configuration wizard will ask you to provide the configuration parameters below

* Index to send data to
* Comma separated list of Splunk Indexer URI's - Host:Port e.g. idx1:9997,idx2:9997
* Workers - To scale up forwarding you can launch with multiple workers
* Version - The version of the forwarder to use. Apica can release new versions of the forwarder over time with newer capabilities.&#x20;
  * Latest version of plugin is **logiqai/hauler-splstos:v0.6**

![](<../../.gitbook/assets/image (6).png>)

![Forwarder Proxy configuration to a list of indexer instances](<../../.gitbook/assets/Screen Shot 2022-08-01 at 9.21.30 PM.png>)
