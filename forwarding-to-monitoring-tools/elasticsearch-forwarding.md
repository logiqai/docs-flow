---
description: This page explains how to forward logs to New Relic from LOGIQ.AI
---

# Elasticsearch Forwarding

To Generate API Key from Elasticsearch, please follow the instructions in this [link](https://www.elastic.co/guide/en/elasticsearch/reference/current/security-api-create-api-key.html).

## Steps to Create Elasticsearch Forwarding

To forward your logs to Elasticsearch, begin by logging into LOGIQ.AI's website.

* Navigate to the **`Create`** tab and select the option for **`Forwarder`**.
* Next, choose **`Dynatrace(HTTP event collector)`** from the available options; this will bring up a new form with fields such as `API Key`, `Host`, `Tags`, etc. Fill out the required data in these fields and click **`Create`**.

Create Forwarder:

<pre><code><strong>Api_Key:       &#x3C;DYNATRACE-API-KEY>
</strong>Host:          &#x3C;DYNATRACE-ENDPOINT>
Tags:          logflow
Type:          _json
Name:          Dynatrace
</code></pre>

* Next, head over to the **`Explore`** page and pick out a namespace you wish to forward your logs to Dynatrace from.
* Click on the three dots icon located next to the calendar and opt for **`Map Forwarder`**; this will open a new modal which allows you to choose the newly created Dynatrace forwarder schema (this can be identified via its Dynatrace icon).
* Confirm your selection by clicking **`OK`**.
* A successful mapping is indicated by a popup showing that namespace-application pairs are connected with respective forwarders; additionally, you'll notice an updated Namespace Forwarder status in effect.
* Your logs are now being forwarded to Dynatrace.

> To help make the steps easier to understand, below are the screenshots illustrating each of the instructions given above.
