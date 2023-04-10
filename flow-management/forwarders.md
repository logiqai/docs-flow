# Forwarders

**LOGIQ** provides multiple targets to connect with your desired destination to collect, optimize, store, route, and replay your observability data – whenever, wherever you need it.&#x20;

Currently, **LOGIQ** supports the below targets

|                                                        Target                                                       |        Type        |                     Description                     |
| :-----------------------------------------------------------------------------------------------------------------: | :----------------: | :-------------------------------------------------: |
|                [ArcSight Logger](https://logflow-docs.logiq.ai/security-monitor-forwarding/arc-sight)               |  Syslog, TCP, CEF  |            Forward syslog frames over TCP           |
|                [ArcSight Logger](https://logflow-docs.logiq.ai/security-monitor-forwarding/arc-sight)               |     Syslog, TCP    |         Forward ArcSight CEF frames over TCP        |
|              [DataDog](https://logflow-docs.logiq.ai/forwarding-to-monitoring-tools/datadog-forwarding)             |        JSON        |        Batched JSON forward to DataDogDataDog       |
| [Dynatrace HTTP Event Collector](https://logflow-docs.logiq.ai/forwarding-to-monitoring-tools/dynatrace-forwarding) |        JSON        |          Batched JSON forward to Dynatrace          |
|     [Elastic Compatible](https://logflow-docs.logiq.ai/forwarding-to-monitoring-tools/elasticsearch-forwarding)     |        JSON        |            Send data to an Elastic index            |
|          [RSA NetWitness Syslog](https://logflow-docs.logiq.ai/security-monitor-forwarding/rsa-new-witness)         |         TCP        |         Syslog forwarder for RSA Netwitness         |
|       [RSA NetWitness Syslog (CEF)](https://logflow-docs.logiq.ai/security-monitor-forwarding/rsa-new-witness)      |      TCP, CEF      |       Syslog CEF forwarder for RSA Netwitness       |
|  [NewRelic HTTP Event Collector](https://logflow-docs.logiq.ai/forwarding-to-monitoring-tools/new-relic-forwarding) |        JSON        |           Batched JSON forward to NewRelic          |
|                                             Splunk HTTP Event Collector                                             |        JSON        |            Batched JSON forward to Splunk           |
|                                         Splunk Universal  / Heavy Forwarder                                         |     Syslog, TCP    |             Syslog forwarder for Splunk             |
|                                            Splunk Universal CEF Forwarder                                           |  Syslog, TCP, CEF  |           Syslog CEF forwarder for Splunk           |
|                                     Splunk Universal Forwarder / Heavy Forwarder                                    |         S2S        |       Forward data to LOGIQ.AI in Cooked mode       |
|                 [Object Store ](https://logflow-docs.logiq.ai/object-store-forwarding/s3-compatible)                |    S3 Compatible   | AWS S3, CEPH, Minio, GCP Cloud Storage, OCI Buckets |
|               [Object Store](https://logflow-docs.logiq.ai/object-store-forwarding/azure-blob-storage)              | Azure Blob Storage |     Native support for Azure blob storage API's     |

### Configuring a Forwarder

To configure a Forwarder navigate to the Forwarder page first and Select your preferred forwarder

Below, an example of configuring a Splunk HTTP Event Collector is shown

1.  **Creating an HTTP Event Collector Data Input key from Splunk**

    * Navigate to your Splunk Environment&#x20;
    * Locate the Settings menu
    * Locate the Data Inputs sub-menu
    * Click on the New Token option which is located on the top banner
    * Enter a Token name and skip to the last page and click Done&#x20;
    * Use the generated **HTTP Event Collector** key in LOGIQ


2.  **Creating a Splunk HTTP Event Collector on LOGIQ**

    * Navigate to the Creaet Forwarders page
    * Click on Forwarders
    * Click on the Splunk HTTP Event Collector



    <figure><img src="../.gitbook/assets/Screen Shot 2023-01-02 at 5.31.52 PM.png" alt=""><figcaption><p>Create Forwarder</p></figcaption></figure>

![](<../.gitbook/assets/Screenshot from 2022-07-15 18-18-28.png>)

* Fill out all the below fields and click save
  * **buffer\_size**: The Buffer size for logs
  * **host**: Splunk Endpoint
  * **password**: Data Input Key created in step 1
  * **port**: Splunk server receiving port (default 8088)
  * **type:** log format (_default_ \__json, or set to \_metric to send to a metric index_)
  * **user:** UI username of Splunk Endpoint
  * **name**: Name of the forwarder&#x20;

![](<../.gitbook/assets/2022-07-15\_18-42 (1).png>)

That's it. You've successfully created the Splunk HTTP Event Collector forwarder. Now navigate to the Explore page and start doing Mapping or Replay operation.&#x20;
