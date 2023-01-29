Topic: GitHub Actions Best Practices 1
Date: Jun 2, 2022
Course: N/A
Class: N/A

---

### Questions/Cues
- What can we do at the [[UDRC]] with [[GitHub]] and [[GitGuardian]] to improve our build security?

### Notes
- [[tokens]] should have least-required permissions
- [[actions]] can have version tags and their run/property state recorded
- do not [[echo]] values we do not explicitly control or set.  use intermediate environment variable.
- Workflows need to be run on trusted code and only executed when expected.
- Self-hosted runners are a big security hole.  Pay GitHub for more actions!
- [[OIDC]] [[OpenID Connect]] is the preferred way to access cloud resources
- 

### Summary
Highlight ==best practices are for everyone. use the scanning, but be careful with secrets==
```
Security.md - do not use any self identifying information not shared by the organization (name is ok)

OICD connections are not currently in use across all our repositories.  On moving to USHE, a question of SSO accessability to resources will be an issue.  We may be able to integrate USHE OICD into our GitHub actions pipelines.  An interesting consideration for synergizing user access management with more general build/agent access.
```