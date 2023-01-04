# Overview

LOGIQ.AI's plugins include creating one or more Splunk Output configurations that can be then used to send data to Splunk. We support all the enterprise modes for forwarding, including sending data to a Standalone Server, a list of indexers, and sending data to indexers using Peer discovery.

### Architecture

<figure><img src="../.gitbook/assets/splunk-arch.png" alt=""><figcaption><p>LOGIQ Splunk Forwarding components</p></figcaption></figure>

The Splunk plugin for output configurations can be launched from the _App Extensions_ section under _Explore_.

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-02 at 5.25.13 PM.png" alt=""><figcaption></figcaption></figure>

Selecting the _"Forwarding Proxy"_ app, gives you the configured proxies as well as the ability to create a new one.

![List of configured Splunk Forwarding Proxies](<../.gitbook/assets/Screen Shot 2022-08-01 at 9.20.16 PM.png>)

You can expand on the proxy to see its settings. The "hec\_token" can be used to setup the forwarder.

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-04 at 1.45.42 PM.png" alt=""><figcaption></figcaption></figure>

![Proxy Settings](<../.gitbook/assets/Screen Shot 2022-08-01 at 9.20.44 PM.png>)
