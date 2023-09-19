---
description: This page explains how to forward logs to New Relic from Apica
---

# Elasticsearch Forwarding

To Generate API Key from Elasticsearch, please follow the instructions in this [link](https://www.elastic.co/guide/en/elasticsearch/reference/current/security-api-create-api-key.html).

## Steps to Create Elasticsearch Forwarding

To forward your logs to Elasticsearch, begin by logging into Apica's website.

* Navigate to the **`Create`** tab and select the option for **`Forwarder`**.
* Next, choose **`Elasticsearch(HTTP event collector)`** from the available options; this will bring up a new form with fields such as `API Token`, `Buffer Size`, `Index`, etc. Fill out the required data in these fields and click **`Create`**.

Create Forwarder:

<pre><code><strong>Apitoken:      &#x3C;ELASTIC-API-KEY>
</strong>Buffer_size:   20000
Index:         &#x3C;INDEX-NAME>
Password:      &#x3C;PASSWORD>
Type:          _json
Urls:          &#x3C;ELASTIC-ENDPOINT>
User:          &#x3C;USERNAME>
Name:          Elasticsearch
</code></pre>

* Next, head over to the **`Explore`** page and pick out a namespace you wish to forward your logs to Elasticsearch from.
* Click on the three dots icon located next to the calendar and opt for **`Map Forwarder`**; this will open a new modal which allows you to choose the newly created Elasticsearch forwarder schema (this can be identified via its Elasticsearch icon).
* Confirm your selection by clicking **`OK`**.
* A successful mapping is indicated by a popup showing that namespace-application pairs are connected with respective forwarders; additionally, you'll notice an updated Namespace Forwarder status in effect.
* Your logs are now being forwarded to Elasticsearch.

> To help make the steps easier to understand, below are the screenshots illustrating each of the instructions given above.

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-23-05.png" alt=""><figcaption><p>Forwarders List (Create -> Forwarder)</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-23-11.png" alt=""><figcaption><p>New Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-23-39.png" alt=""><figcaption><p>Create Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-23-49.png" alt=""><figcaption><p>Select a Namespace</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-24-25.png" alt=""><figcaption><p>Map Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-24-42.png" alt=""><figcaption><p>Selecting Elasticsearch schema</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 19-25-05.png" alt=""><figcaption><p>Successful mapping</p></figcaption></figure>
