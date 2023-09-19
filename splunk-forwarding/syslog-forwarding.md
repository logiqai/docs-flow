# Syslog forwarding

You can also create a forwarder to send data in syslog format to Splunk. Note his needs you to enable the syslog receive ports on the Splunk instance

There are two types for syslog forwarding that are supported

1. Raw Syslog
2. Syslog CEF

{% hint style="info" %}
Apica does not support sending to syslog UDP ports. Only TCP ports are supported.
{% endhint %}

Create the appropriate forwarder type when creating the forwarder

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-04 at 2.31.48 PM.png" alt=""><figcaption><p>Splunk Forwarder Syslog / CEF</p></figcaption></figure>

Once selected, provide the syslog port details for sending the syslog data

<figure><img src="../.gitbook/assets/Screen Shot 2023-01-04 at 2.28.38 PM.png" alt=""><figcaption><p>Syslog configuration</p></figcaption></figure>
