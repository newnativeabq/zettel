Topic: Pattern Mining and Detection of Malicious SQL Queries on Anonymization Mechanism
Date: Jul 3, 2022

[[Pattern_Mining_and_Detection_of_Malicious_SQL_Queries_on_Anonymization_Mechanism.pdf]]
---

### Questions/Cues
- How do we detect malicious SQL?

### Notes
- Tradeoffs between "...the privacy and utility of personal data."
- Context of data anonymization techniques (masking, fuzzing).
	- [[k-anonymous]] : database reconstruction risk
	- [[differential privacy]]: utility constrained (lots of noise when data is small?), [[inference attacks]]
	- [[Diffix]]: unlimited queries may lead to enough sampling to remove noise.  Used as base for paper
	- They achieved a natural language classifier (random forest?) able to perform detection of many malicious queries
	- BigQuery queries are submitted as web request.  Is it safe to assume that Google is handling detection of a number of attacks?  Maybe, maybe not.
	- Attack Types:
		- [[averaging attack]]: repeat one query, average results to approximate true result
		- [[differential attack]]: two query conditions differ by only one attribute, resulting in a difference inferring a value
		- [[cloning attack]] multiple query statements with same syntax and dummy conditions are used to sample out individual level data
		- [[linear reconstruction attack]]: multiple sets of queries with non-intersecting query ranges and dummy conditions issued to obtain noise samples and recreate database

### Summary
Highlight ==what’s important!==
```
The UDRC cannot add noise to researcher's data at this time.  The impact to their analysis would have to be rigrously explored.  

A query analyzer to detect malicious SQL statements and set of rules specific to Indexed data may be easier to implement and more immediately protective.
```