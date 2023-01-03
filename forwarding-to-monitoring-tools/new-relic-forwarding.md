---
description: This page explains how to forward logs to New Relic from LOGIQ.AI
---

# New Relic Forwarding

To Generate API Key from New Relic, please follow the instructions in this [link](https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/#setup).

## Steps to Create New Relic Forwarding

To forward your logs to New Relic, begin by logging into LOGIQ.AI's website.

* Navigate to the **`Create`** tab and select the option for **`Forwarder`**.
* Next, choose **`New Relic (HTTP event collector)`** from the available options; this will bring up a new form with fields such as `API Key`, `Host`, `Tags`, etc. Fill out the required data in these fields and click **`Create`**.

Create Forwarder:

<pre><code><strong>Api_Key:       &#x3C;NEW-RELIC-API-KEY>
</strong>Host:          log-api.newrelic.com
Tags:          logflow
Type:          _json
Name:          New Relic
</code></pre>

* Next, head over to the **`Explore`** page and pick out a namespace you wish to forward your logs to New Relic from.
* Click on the three dots icon located next to the calendar and opt for **`Map Forwarder`**; this will open a new modal which allows you to choose the newly created New Relic forwarder schema (this can be identified via its New Relic icon).
* Confirm your selection by clicking **`OK`**.
* A successful mapping is indicated by a popup showing that namespace-application pairs are connected with respective forwarders; additionally, you'll notice an updated Namespace Forwarder status in effect.
* Your logs are now being forwarded to New Relic.

> To help make the steps easier to understand, below are the screenshots illustrating each of the instructions given above.

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 15-00-19.png" alt=""><figcaption><p>Creating New Forwarder from <strong><code>Create -> Forwarder</code></strong> page</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 15-01-00.png" alt=""><figcaption><p>Create Forwarder Modal</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 15-01-23.png" alt=""><figcaption><p>Explore page selecting a namespace</p></figcaption></figure>



<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 15-01-32.png" alt=""><figcaption><p>Map Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 15-01-45.png" alt=""><figcaption><p>Selecting New Relic Forwarder Schema from Dropdown</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 15-01-55.png" alt=""><figcaption><p>Success message after a successful mapping</p></figcaption></figure>
