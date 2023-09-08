---
description: >-
  This page explains how to forward logs to Azure Log Analytics from Apica
  Ascent
---

# Azure Log Analytics Forwarding

You can forward your logs to the Azure log analytics platform. This will enable you to run queries on our log data which will provide more insights from your data.

### Prerequisite

* Azure log analytics workspace

### Create Log Analytics Forwarder

* Navigate to the integrations page and select the forwarders tab

<figure><img src="../.gitbook/assets/Screenshot from 2023-09-07 18-26-51.png" alt=""><figcaption></figcaption></figure>

* Click on the "Add Forwarder" Button and select Log analytics



<figure><img src="../.gitbook/assets/Screenshot from 2023-09-07 18-32-32 (1).png" alt=""><figcaption></figcaption></figure>

* Provide the `workspace id` of your Log Analytics workspace
* Provide the `Shared Key` from your Log Analytics workspace. This can be found under the agents menu in log analytics
* Select the log type\
  \
  If `Use source type in log as log type` is selected, then the value in the source type attribute from your log will be used as a custom table name. For example, if your log has source\_type  `fluent bit` then those logs will be stored under `fluent bit` table in your log analytics workspace.\
  \
  If `Provide log type manually` is selected, then you should provide the log type manually in the `Custom log type` text field.



<figure><img src="../.gitbook/assets/Screenshot from 2023-09-07 18-35-03.png" alt=""><figcaption></figcaption></figure>

* You can choose whether you want to send filtered data or raw data to your forwarder by providing the boolean value in `Filter Forward` field
* Provide a name for the forwarder
* Click on Create\


After creating the log analytics forwarder, it can be mapped to any namespace and application. Your Log Analytics workspace will get the data once the logs are ingested into the namespace/application that is mapped.

