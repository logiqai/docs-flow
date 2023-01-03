---
description: Google Pub/Sub is the GCP managed service for real-time stream processing
---

# Google Pub/Sub

LOGIQ.AI's LogFlow can be used to push data to a PubSub topic with just a few clicks. You can forward data as is, morph the data by stripping down attributes or pick and choose the fields that you want to be sent to the Google PubSub topic

### Pre-requisites

You will need the following before you can configure forwarding to Google PubSub

1. Name of the Google PubSub topic
2. Project id ( full name not an integer ) for your GCP account project where you created the topic
3. Service account access JSON

{% hint style="info" %}
The service account must have _<mark style="color:purple;">**pubsub.topics.publish**</mark>_ permissions
{% endhint %}

You can check your service account json permissions with gcloud cli&#x20;

```bash
$ gcloud auth activate-service-account --project=my-project-123 \
--key-file=sevice_account_key_file.json
$ gcloud pubsub topics publish my-gcp-topic-1 --message="hello"
messageIds:
- '6470211179713996'
$ gcloud pubsub subscriptions pull my-gcp-topic-1-sub --auto-ack
┌───────┬──────────────────┬──────────────┬────────────┬──────────────────┐
│  DATA │    MESSAGE_ID    │ ORDERING_KEY │ ATTRIBUTES │ DELIVERY_ATTEMPT │
├───────┼──────────────────┼──────────────┼────────────┼──────────────────┤
│ hello │ 6470211179713996 │              │            │                  │
└───────┴──────────────────┴──────────────┴────────────┴──────────────────┘
```

### Creating the forwarder

We are now ready to create the forwarder

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-02 at 12.36.15 PM.png" alt=""><figcaption><p>Create Google PubSub forwarder</p></figcaption></figure>

### Enter forwarder configuration

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-02 at 12.39.03 PM.png" alt=""><figcaption><p>Forwarder configuration</p></figcaption></figure>

### Testing the Google PubSub forwarding

You can now test a data replay with a test stream to see if data went through

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-02 at 12.41.29 PM.png" alt=""><figcaption><p>Replay data to Google PubSub</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-02 at 12.42.16 PM.png" alt=""><figcaption><p>Replay status for Google PubSub forwarded data</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Screen Shot 2022-12-02 at 12.45.22 PM.png" alt=""><figcaption><p>Visualizing data forwarding to Google PubSub</p></figcaption></figure>
