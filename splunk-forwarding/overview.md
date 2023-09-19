# Overview

Apica's plugins include creating one or more Splunk Output configurations that can be then used to send data to Splunk. We support all the enterprise modes for forwarding, including sending data to a Standalone Server, a list of indexers, and sending data to indexers using Peer discovery.

### Architecture

<figure><img src="../.gitbook/assets/splunk-arch (1).png" alt=""><figcaption><p>Splunk S2S Forwarding architecture</p></figcaption></figure>

### Required components

Follow the below steps to create an S2S forwarder to a splunk indexer

1. Create a UF Proxy app extension
2. Create a forwarder to use the UF proxy app extension created in step 1 above
   * One or more forwarders can be created to use the same UF Proxy app
     * Forwarders can be of type \__json or \_metric_&#x20;
     * \_metric type can forward to a splunk metric index
     * \_json can forward to a splunk standard index

### Creating UF proxy app extension

The Splunk plugin for output configurations can be launched from the _App Extensions_ section under _Explore_.

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-02 at 5.25.13 PM.png" alt=""><figcaption></figcaption></figure>

Selecting the _"Forwarding Proxy"_ app gives you the configured proxies as well as the ability to create a new one.

![List of configured Splunk Forwarding Proxies](<../.gitbook/assets/Screen Shot 2022-08-01 at 9.20.16 PM.png>)

You can expand on the proxy to see its settings. The "hec\_token" can be used to setup the forwarder.

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-04 at 1.45.42 PM.png" alt=""><figcaption></figcaption></figure>

![Proxy Settings](<../.gitbook/assets/Screen Shot 2022-08-01 at 9.20.44 PM.png>)
