[[messaging]] [[security]]

# Secure Messaging Intra/Inter/Ex in GCP
All cross project communication originating in a C2 or C1 project needs to be scanned before delivery.

## Secure Messaging Workflow
The SLDS secure messaging workflow will specify how C1, C2 projects communicate with the outside world and each other.

All messages, regardless of size or deliverable, will go through screening. 

emitter (client) -> screen -> pub/sub

This means all messages need:

1. topic?
2. key?
3. body?


### Screening Messages
All messages are screened via data loss prevention (DLP) scanner.


## References
1. [Google Cloud Sensitive Data and ML Datasets](https://cloud.google.com/architecture/sensitive-data-and-ml-datasets)