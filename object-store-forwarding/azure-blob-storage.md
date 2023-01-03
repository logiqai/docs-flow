# Azure Blob Storage

## Pre-requisite

* Azure blob store for storing logs
* Account key and account name which will have permission to upload objects to the blob store

## Steps for Creating Azure Blob Forwarding

* Navigate to `Create Forwarder` page
* Select Azure Blob Store
* Click `New Forwarder` button
* Provide forwarder name
* Provde Account name, account key, container name (bucket name) and endpoint for azure blob store
* Click `Create` button

<figure><img src="../.gitbook/assets/Screenshot from 2023-01-03 01-11-47.png" alt=""><figcaption></figcaption></figure>

The Azure Blob store Forwarder can now be mapped to any data flow. The Azure blob store forwarder breaks the data into smaller objects based on the object size configuration. The default object size is set to 4MB and can be changed while creating the forwarder.
