```
# USIS - Student Challenge Session

Date: Sep 21, 2022
Attendees:
Jeremias Solari
Vincent Brandon
---

# Goals / agenda
1. Begin condensing value options for data system expansion under USIS

# Discussion notes
- 

# Action items
- [ ] Meeting Notes Distributed to the Team
- [ ] Tasks & Projects Completed, Processed or Delegated
- [ ] Key Dates Completed or Scheduled
```

[[USIS]]
Putting it all together:

USIS - The Universal Student Identification System is a:
1. Student Challenge Agent [single user]- students may provide mixed sensitive information to authenticate/authorize retrieval of specific sensitive fields if available.  Returns index information retrieval authorization token.
2. Application Challenge Agent [application user] - applications may request batch challenges for large searches of available records. Returns index information retrieval authorization token(s).
3. General Query Engine [ single/application user(s)] - return field data if authorized and available for given authorization token index identifier.


To deploy:
A.1 Create USIS challenge and batch agents with Master Person Index pool & class 1 data pointers
A.2 Create API service wrapper to manage USIS as sharable resource
A.3 Create service sharing platform behind Google IAM to configure resource access
A.3.I Create SLDS Resource Clearinghouse Frontend
A.3.II Create SLDS Resource Clearinghouse Backend Infrastructure
B. Create population service that creates a how-to from USIS API or manual entry to create resource access instructions in SLDS Frontend dashboard (consumer)
C. Configure API gateway to allow resource passthrough

Name Ideas for SLDS Resource Clearinghouse:
[[Aspen]] [[aspen]]
Utah national tree: https://www.google.com/search?q=utah+national+tree&rlz=1C1GCEA_enUS1022US1022&ei=UEYrY9SIL8nWkPIP_fivsAI&ved=0ahUKEwjU8LeNsab6AhVJK0QIHX38CyYQ4dUDCA4&uact=5&oq=utah+national+tree&gs_lcp=Cgdnd3Mtd2l6EAMyBggAEB4QFjIGCAAQHhAWMgYIABAeEBYyBggAEB4QFjIGCAAQHhAWMgYIABAeEBYyBggAEB4QFjIGCAAQHhAWMgYIABAeEBYyBggAEB4QFjoKCAAQRxDWBBCwAzoCCCY6CAgAEIAEELEDOgUIABCABDoLCC4QxwEQrwEQkQI6CwguEIAEEMcBEK8BOggIABAeEA8QFkoECEEYAEoECEYYAFCcBViuD2CWEGgBcAF4AIABlAGIAYwHkgEDMS43mAEAoAEByAEIwAEB&sclient=gws-wiz