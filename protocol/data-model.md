# Clarus Protocol — Data Model

Version 0.1

This document defines the core data structures used by the Clarus Protocol.

The model is designed around one principle:

> Verify, do not trust.

The protocol records public information in a structured, auditable format while minimizing personal data.

---

## 1. Government Entity

Represents a public institution or government body.

```text
GovernmentEntity
- entity_id
- country
- jurisdiction
- entity_type
- name
- parent_entity_id
- official_source
- active_from
- active_to
