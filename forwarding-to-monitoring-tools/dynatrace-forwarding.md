---
description: This page explains how to forward logs to Dynatrace from Apica.
---

# Dynatrace Forwarding

To Generate an API Key from Dynatrace, please follow the instructions in this [link](https://www.dynatrace.com/support/help/dynatrace-api/basics/dynatrace-api-authentication).

## Steps to Create New Relic Forwarding

To forward your logs to Dynatrace, begin by logging into Apica's website.

* Navigate to the **`Create`** tab and select the option for **`Forwarder`**.
* Next, choose **`Dynatrace(HTTP event collector)`** from the available options; this will bring up a new form with fields such as `API Key`, `Host`, `Tags`, etc. Fill out the required data in these fields and click **`Create`**.

Create Forwarder:

<pre><code><strong>Api_Key:       &#x3C;DYNATRACE-API-KEY>
</strong>Host:          &#x3C;DYNATRACE-ENDPOINT>
Tags:          logflow
Type:          _json
Name:          Dynatrace
</code></pre>

* Next, head over to the **`Explore`** page and pick out a namespace you wish to forward your logs to Dynatrace.
* Click on the three dots icon located next to the calendar and opt for **`Map Forwarder`**; this will open a new modal that allows you to choose the newly created Dynatrace forwarder schema (this can be identified via its Dynatrace icon).
* Confirm your selection by clicking **`OK`**.
* A successful mapping is indicated by a popup showing that namespace-application pairs are connected with respective forwarders; additionally, you'll notice an updated Namespace Forwarder status in effect.
* Your logs are now being forwarded to Dynatrace.

> To help make the steps easier to understand, below are the screenshots illustrating each of the instructions given above.

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 17-54-30.png" alt=""><figcaption><p>List of Forwarders</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 17-54-43.png" alt=""><figcaption><p>Create Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 17-55-41.png" alt=""><figcaption><p>Selecting a Namespace</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 17-55-50.png" alt=""><figcaption><p>Map Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 17-56-17.png" alt=""><figcaption><p>Selecting Dynatrace forwarder schema as Forwarder</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 17-56-30.png" alt=""><figcaption><p>Successful Mapping of Forwarder</p></figcaption></figure>
