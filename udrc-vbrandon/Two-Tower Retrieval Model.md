Topic: Two-Tower Retrieval Model
Date: Jul Th, 2022; 2022-07-28
Detail:  Recommender architecture
https://cloud.google.com/vertex-ai/docs/matching-engine/train-embeddings-two-tower
---
[[AI]] [[recommender]] [[algorithm]]

[[A Dual Augmented Two-Tower Model for Online Large-scale Recommendation.pdf]]

### Questions/Cues
- What makes this architecture useful? When?
- What needs to be understood about this architecture to minimally implement a mild production system?

### Notes
- The goal of the two tower approach is to take related document classes and embed them into the same vector space for nearest neighbor approximations.  The 'user-preference' query document is close to these 'candidate-item' documents.
- 

### Summary
Highlight ==what’s important!==
```
An augmented two tower model, though potentially leading to improved results, is overkill for our little system (not enough sparsity to care?)
```