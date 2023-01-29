# UDRC Infrastructure Deployment Milestone Report
2022-09-29

## Data Systems Overview
[[GCP Tenant]]
- [[Access & Structure]]
- - SLDS & Burwood Staff developer and researcher permissions allow work across projects
- - Project structure, permissions, and repository connections established for:
- - - web-udrc-main
*notes: connected via cloudbuild, infrastructure-deployment*
**status** milestone complete. internal development underway.
- - - mpi-udrc-gcp
*notes: connected via cloudbuild, infrastructure-deployment*
**status** milestone complete. internal development underway.
- - - gcp-infrastructure-deployment (readiness tbd by Burwood)
*notes: functioning deployment of proscribed project structure.*
**status** milestone complete.  security controls require updates to Google Security Command Center.
- - - webteam-udrc-admin-api
*notes: connected via cloudbuild, infrastructure-deployment. login pending.*
**status** milestone complete. development pending application database launch.
- - - webteam-udrc-admin-client
*notes: connected via cloudbuild, infrastructure-deployment. login pending.*
**status** milestone complete. development pending application database launch.
- - - webteam-udrc-researcher-api
*notes: connected via cloudbuild, infrastructure-deployment. login pending.*
**status** milestone complete. development pending application database launch.
- - - webteam-udrc-researcher-client
*notes: connected via cloudbuild, infrastructure-deployment. login pending.*
**status** milestone complete. development pending application database launch.

[[Active Deployment]]
- [[UDRC Main Site]]
- - Live at IP
- - .io DNS routes reach development, production, load balancers
- - github integration development, production
*notes: development (dev.udrc.io) and production (udrc.io) successfully diverged*
**status** milestone complete. development workflows successfully implemented.

- [[Researcher Workspace]]
- - BigQuery query of c2 (de-identified) data returns results
*notes: results returned.  automatic data (table metadata) discovery limited.
**status** milestone complete.  workflows in development.

### Follow Up Questions
udrc-p vs. udrc-s project designations.  Raw projects with 'p' designation?

Baseline looks great.  Dev still in sandbox?  That's ok for today.  I'll just make a note.