# Clarus Protocol — Data Model

Version 0.1

The Clarus Protocol uses structured records to make public information traceable, auditable, and independently verifiable.

## 1. Government Entity

- entity_id
- country
- jurisdiction
- entity_type
- name
- parent_entity_id
- official_source

## 2. Public Budget

- budget_id
- government_entity_id
- fiscal_year
- program_id
- category
- approved_amount
- currency
- approval_date
- official_source
- source_hash

## 3. Public Contract

- contract_id
- government_entity_id
- procurement_id
- title
- description
- procedure_type
- publication_date
- award_date
- contract_start
- contract_end
- awarded_amount
- currency
- supplier_id
- number_of_bidders
- official_source
- source_hash

## 4. Supplier

- supplier_id
- legal_name
- country
- registration_id
- incorporation_date
- official_registry_source
- source_hash

## 5. Payment

- payment_id
- contract_id
- government_entity_id
- supplier_id
- payment_date
- amount
- currency
- payment_type
- invoice_reference
- official_source
- source_hash

## 6. Public Project

- project_id
- contract_id
- project_type
- location
- description
- planned_start
- planned_end
- actual_start
- actual_end
- planned_cost
- final_cost
- completion_status
- evidence_source

## 7. Public Official

- official_id
- government_entity_id
- role
- start_date
- end_date
- compensation
- compensation_period
- official_source
- source_hash

## 8. Public Promise

- promise_id
- actor_id
- jurisdiction
- statement
- publication_date
- source
- target_date
- status
- evidence
- last_verified

Possible statuses:

- PROPOSED
- IN_PROGRESS
- DELIVERED
- DELAYED
- CHANGED
- REVERSED
- NOT_DELIVERED
- UNVERIFIED

## 9. Audit Signal

- signal_id
- object_type
- object_id
- rule_id
- severity
- generated_at
- evidence
- uncertainty
- review_status
- response

An audit signal is NOT proof of wrongdoing. It identifies a pattern that may require human investigation.

## 10. Source

- source_id
- institution
- dataset
- publication_url
- publication_date
- retrieval_date
- format
- source_hash
- verification_status

## 11. Evidence

- evidence_id
- object_type
- object_id
- source_id
- evidence_type
- reference
- hash
- timestamp

## 12. Vote Eligibility

- election_id
- polling_station_id
- anonymous_credential
- eligibility_verified
- ballot_issued
- timestamp

The system must not publicly link a person's identity to their vote.

## 13. Anonymous Vote

- election_id
- anonymous_vote_id
- ballot_commitment
- vote_proof
- timestamp

The vote must not contain personally identifying information.

## 14. Physical Ballot

- election_id
- ballot_hash
- polling_station_id
- audit_batch
- counted

The physical ballot provides an independent paper audit trail.

## 15. Election Reconciliation

The voting system reconciles:

1. Verified voters
2. Ballots issued
3. Digital votes
4. Physical paper ballots

The identity of a voter must remain separated from their vote.

## 16. Integrity

Important records may be hashed before being committed to the public ledger.

A hash can show that data was not silently modified after publication.

A hash does NOT prove that the original information was truthful.

## 17. Privacy

Public information → Open by default

Personal information → Minimize

Sensitive information → Protect

Identity ↔ Vote choice → Never publicly link

## 18. Verification Status

- UNVERIFIED
- SOURCE_VERIFIED
- CROSS_VERIFIED
- AUDITED
- DISPUTED
- SUPERSEDED

## 19. Core Public-Money Chain

Budget
↓
Procurement
↓
Contract
↓
Payment
↓
Project
↓
Evidence

The purpose is to allow citizens to follow public money from authorization to expenditure to result.

## 20. Design Rule

Clarus does not ask citizens to trust the system simply because information is recorded in it.

The protocol provides:

- Traceability
- Integrity
- Evidence
- Independent verification
- Auditability

It does not replace human judgment, independent institutions, courts, auditors, journalists, or citizens.
