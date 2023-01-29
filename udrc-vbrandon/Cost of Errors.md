Topic: Cost of Errors
Date: Jul We, 2022; 2022-07-27
Detail: Context dependent cost of errors in ML decision making systems

---
[[machine learning]] [[error]] [[cost]] [[ML]] [[decisions]]
### Questions/Cues
- How does the cost of model error against the RWF (real world function) impact the utility and development of the model?


### Notes
- Accuracy measures the difference between a machine learning model and an observed function (data); however, observed functions (OF) are samples of real world functions (RWF).
- This can create a cost avoidance loop meaning ml system outputs do not get tested against the real world and the training hits a plateau based on the available sample data showing the OF

### Summary
Highlight ==what’s important!==
```
By adding in a compensation system to the decision-making pipeline, the total cost of decisions is C = cost of error + cost of compensation.  This can be minimized and compensation becomes a better reflection of RWF - OF.
```

