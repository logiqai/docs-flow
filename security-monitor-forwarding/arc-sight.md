# Arc Sight

ArcSight is a security management tool designed to track and analyze data insights and it ensures compliance with policy guidelines. It provides organizations with the real-time security information that can be used to detect and respond to threats quickly and effectively.

LogiqAI helps you to forward logs to the arc sight using the forwarder plugin.

## Supported Forwarding Formats

LogiqAI enables users to quickly and easily forward logs in various formats to security tools, simplifying processing and analysis. The supported formats are,

* Syslog CEF
* ArcSight CEF

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 14-36-35.png" alt=""><figcaption></figcaption></figure>

## Steps to Create Arc Sight Forwarding

* Expand the `Create` menu from the navigation bar and click `Forwarder`&#x20;
* Select the `Arc Sight` based on the type of format you want to use
* Click `New Forwarder` button at the top right corner
* Provide the host of the Arc Sight and the name of the forwarder
* Click `Create`

Once the forwarder is associated with a specific namespace/application or with various log attributes, the logs that match these criteria will be sent to ArcSight for further analysis.

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 14-23-56.png" alt=""><figcaption><p>creating arc sight forwarder</p></figcaption></figure>

