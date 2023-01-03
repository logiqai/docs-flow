# Standalone Instance

You can launch the proxy to forward data to a Splunk standalone instance. The proxy configuration wizard will ask you to provide the configuration parameters below

* Index to send data to
* Standalone Splunk instance URI - Host:Port e.g. mysplunk.instance:9997
* Workers - To scale up forwarding you can launch with multiple workers
* Version - The version of the forwarder to use. LOGIQ.AI can release new versions of the forwarder over time with newer capabilities.
  * Latest version of plugin is **logiqai/hauler-splstos:v0.6**

![](<../.gitbook/assets/image (4).png>)

![Scale out Forwarding cluster for Standlone Splunk setup](<../.gitbook/assets/Screen Shot 2022-08-01 at 9.21.52 PM.png>)

