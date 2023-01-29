# Universal Student Identification System (USIS)
Currently, students are being authorized with a large amount of PII and real-time checks with sensitive databases at USBE and USHE institutions.  The State Longitudinal Data System [[slds]] could provide a single source authentication system for students needing to authorize with arbitrary sensitive fields across multiple contexts.

E.g.
- A k-12 student needs to authorize multiple USBE institutions to send transcripts, can authenticate as a student across all of them at once with either:
	- k-12 Personally identifiable information (PII collected at k-12 institutions)
	- Partner-specific identifying information (Authenticate through college email system and get back student ID or other 'safe' identifiers)
	- Partner-specific personally identifiable information (PII collected at partner institution)

## Why this works
The SLDS master person indexing and de-identification systems maintains a virtual identity pool that aggregates PII (or pointers to PII) across all our partner data sets.  This allows authentication proofs to be designed to check against a inter-agency set of identifying information, proving validity at system confidence, that an entity static across multiple partners.  

Another way to state this might be that we can design proofs and then authentication schemes that work for students and data partners with the data clients and client-engagement systems are expected to have, instead of requiring an arbitrary set of PII be available to the student or staff user.