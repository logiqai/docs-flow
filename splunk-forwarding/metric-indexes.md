# Metric indexes

Apica supports forwarding to splunk metrics indexes. Both old metrics format and new format with multiple metrics per event are supported.

Creating a splunk metrics forwarder is straight forward and uses the _"\_metric"_ type when creating the forwarder

{% hint style="warning" %}
The following formation is obtained from the Apica UF Proxy App extension for the forwarder

1. The **"Host"** key is set to the Apica UF Proxy App extension that was created and should not use the Splunk host name.
2. The **"Password"** is set to the hec\_token from the Apica UF Proxy App extension
3. The **"port"** is set to 8088
4. The **"user"** is set to **"admin"**
{% endhint %}

{% hint style="info" %}
The **Host**, **Password**, **Port**, **User** can also be set to use an external Splunk HEC endpoint directly
{% endhint %}

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-03 at 10.45.54 AM.png" alt=""><figcaption></figcaption></figure>
