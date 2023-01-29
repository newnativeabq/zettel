Topic: GCP - Secure Messaging Whiteboard Session
Date: Oct Mo, 2022; 2022-10-10
Detail:

---

### Questions/Cues
- What could an architecture for secure messaging look like within the secure data enclave
- 

### Notes
- whiteboard session - images annotated below for zettel.  notes in summary.

### Summary
Highlight ==what’s important!==
```
Everything is a file - messages are simple text files with annotations for content source, destination, and operation (see images)

Multi-project system including, but not limited to:
1. email project
2. export project
3. messaging project

on top of SDE and normal operations projects

Users and applications will interface with the messenger through an internally provided standard library in either python or R

Messaging is uniform across sources and destinations regardness of origin or content (same message format for emails and exports)

Process Overview:
1. user/app saves unique blob to project-local outbound bucket
2. user/app-project-local bucket trigger signs message and publishes to pub/sub under topic outbound_messages_raw
3. messaging-project-local trigger calls DLP from Data Ops
4. DLP validates job, checks content, and pushes to pub/sub under topic outbound_email_signed or outbound_file_signed
5. email/export-project-local trigger (subscribed to messaging topic(s)) consume signed message, validate, and process
6. email/export-project-local publishes signed message to either pub/sub topic outbound_messages_complete or outbound_message_retry
```


## Images
[[PXL_20221010_195642145.jpg]]
[[PXL_20221010_195634934.jpg]]
[[PXL_20221010_195651395.jpg]]

### Signatures
application signatures will follow common public key/private key challenge (public key passed with signed message)

#### References
[IBM Public Key Cryptography Explanation](https://www.ibm.com/docs/en/ztpf/1.1.0.14?topic=concepts-public-key-cryptography)
