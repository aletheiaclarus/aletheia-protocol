# The Clarus Protocol

## A verifiable system for citizen voice and public money

**Version 0.2 — September 2026**

Clarus is an open proposal for making public institutions more transparent, auditable, and better managed.

The principle is simple:

> **Verify, do not trust.**

Clarus is designed as a public verification layer for government finances, public contracts, public compensation, political promises, and democratic processes.

It does not replace constitutions, courts, legislatures, governments, or electoral authorities. It provides evidence that citizens, journalists, researchers, auditors, courts, and public institutions can independently verify.

---

## 1. The Problem

Public institutions manage resources that belong to society.

Citizens should be able to understand:

- how public money is collected;
- where it is allocated;
- what contracts are awarded;
- what was paid;
- what was delivered;
- who received public money;
- how public officials are compensated;
- what governments promised;
- what was actually delivered;
- and how democratic decisions were recorded.

Today, this information often exists, but it can be distributed across different systems, institutions, formats, and levels of government.

Clarus proposes a common verification layer that connects these records.

The objective is not to assume that governments are corrupt.

The objective is to make important public actions independently verifiable.

---

## 2. Design Principles

### 2.1 Verify, do not trust

The system should reduce the amount of trust required from citizens.

Important claims should be supported by independently verifiable records.

### 2.2 Open by default

Public information should be publicly accessible unless there is a legitimate legal reason for restricting it.

### 2.3 Minimal personal data

Personal information should not be placed on a public blockchain.

Sensitive information should remain protected.

### 2.4 Independence

The verification infrastructure should not depend exclusively on the government being evaluated.

### 2.5 Evidence before conclusions

Automated systems may identify unusual patterns, but a signal is not an accusation.

Every automated flag should show:

- the rule that generated it;
- the underlying data;
- the source;
- the relevant uncertainty;
- and, where appropriate, the right of reply.

### 2.6 No wealth-based political power

Clarus does not require or create a cryptocurrency.

Voting power must never depend on money, tokens, assets, or ownership.

---

# 3. Public Money Ledger

The Public Money Ledger represents public expenditure as a chain of verifiable events.

A simplified expenditure lifecycle is:

**Budget → Contract → Payment → Result**

Each stage should be independently identifiable.

For example:

1. A public authority approves a budget.
2. A procurement process is published.
3. A contract is awarded.
4. Payments are recorded.
5. The expected result is documented.
6. Completion or delivery is recorded.
7. Evidence supporting completion is retained.

The objective is to allow a citizen to follow public money from authorization to outcome.

---

# 4. Public Contracts

Clarus should connect available official procurement information into a common structure.

A contract record may include:

- contracting authority;
- procurement identifier;
- supplier;
- ownership information where legally public;
- procurement procedure;
- number of bidders;
- awarded amount;
- estimated amount;
- amendments;
- extensions;
- payments;
- delivery milestones;
- completion information.

International standards such as the Open Contracting Data Standard may be used where appropriate.

Country-specific legal systems remain authoritative.

Clarus is a verification layer, not a replacement for official procurement systems.

---

# 5. Automated Audit Signals

Clarus may calculate risk signals from public data.

Examples include:

- a single bidder;
- repeated awards to the same supplier;
- contracts repeatedly amended;
- unusually large cost increases;
- contracts divided into smaller related purchases;
- payments occurring before expected delivery;
- unusually short procurement periods;
- recently created suppliers receiving unusually large contracts;
- relationships between companies receiving repeated awards;
- significant differences between comparable project costs.

These signals do **not** establish wrongdoing.

They identify records that may deserve further examination.

A signal should therefore be displayed as:

**Signal → Evidence → Rule → Context → Verification**

and not as:

**Signal → Accusation**

---

# 6. Construction and Infrastructure

Public infrastructure can be represented as projects with measurable inputs and outputs.

Examples include:

- roads;
- bridges;
- hospitals;
- schools;
- railways;
- metro systems;
- airports;
- ports;
- water infrastructure;
- public housing.

Where reliable comparable information exists, citizens should be able to compare:

- project scope;
- planned cost;
- awarded cost;
- final cost;
- duration;
- amendments;
- quantities;
- geographical conditions;
- and final delivery.

Comparisons must account for legitimate differences between projects.

A higher cost is not automatically evidence of wrongdoing.

---

# 7. Public Compensation

Public compensation should be transparent.

Clarus proposes publishing legally permissible information about:

- senior public officials;
- elected representatives;
- public institutions;
- compensation structures;
- allowances;
- official expenses.

Privacy and security exceptions should apply where disclosure could create a legitimate risk.

The purpose is not to expose individuals unnecessarily.

The purpose is to make the use of public resources understandable.

---

# 8. Government Financial Statement

Government finances should be presented in a form understandable to citizens.

A public financial dashboard may include:

- revenue;
- expenditure;
- assets;
- liabilities;
- debt;
- deficit or surplus;
- cash position;
- major spending categories;
- transfers;
- public investment;
- and changes over time.

The system should allow citizens to move from a high-level figure to the underlying records supporting it.

For example:

**Total infrastructure spending**

→ country

→ region

→ institution

→ project

→ contract

→ payment

→ delivery evidence.

---

# 9. Promise and Performance Ledger

Public promises should be recorded before they disappear from public attention.

A promise record may contain:

- the original statement;
- date;
- source;
- responsible institution or elected official;
- expected deadline;
- measurable objective;
- subsequent changes;
- implementation status;
- evidence of completion.

Possible statuses include:

- Proposed
- In progress
- Completed
- Delayed
- Modified
- Cancelled
- Reversed
- Unable to verify

The system should preserve the original promise.

Later changes should not silently overwrite historical records.

---

# 10. Democratic Accountability

Clarus does not itself remove elected officials.

Constitutions and laws determine how officials may be removed.

Where a jurisdiction legally provides mechanisms such as:

- recall elections;
- referendums;
- votes of no confidence;
- impeachment;
- parliamentary procedures;

Clarus may provide the evidence and verification infrastructure required by those processes.

The protocol must never acquire unilateral political authority.

---

# 11. Voting Protocol

Clarus proposes an auditable voting architecture designed around three independent records:

### A. Voter eligibility and ballot issuance

A legally authorized authority verifies that a person is eligible to vote and that they receive only one voting credential or ballot.

### B. Anonymous physical ballot

The voter casts an anonymous paper ballot.

The paper must not contain:

- the voter's name;
- identification number;
- signature;
- serial number linked to the voter;
- or any other identifier that could reveal the voter's choice.

### C. Digital voting record

The voting system records a cryptographically verifiable representation of the vote without revealing the voter's identity or choice publicly.

These three systems should be independently reconciled.

---

# 12. In-Person Voting

A possible voting procedure is:

1. The voter presents an approved identity document.
2. Eligibility is verified.
3. The voter signs or is recorded in the legally required polling register.
4. The voter receives a one-time anonymous voting credential.
5. The voter enters the voting system.
6. The voter selects their choice.
7. The system records the anonymous digital vote.
8. The voting machine prints a paper representation of the vote.
9. The voter verifies the paper.
10. The voter deposits it into a secure ballot box.
11. The voting credential cannot be used again.

The paper ballot provides an independent audit trail.

---

# 13. Three-Way Reconciliation

After voting closes, three quantities should be reconciled:

**Verified voters / ballots issued**

↔

**Anonymous physical ballots**

↔

**Accepted digital votes**

Any discrepancy must trigger a defined audit procedure.

The digital result must not silently override physical evidence.

The legal rules for resolving discrepancies must be established before an election.

---

# 14. Cryptographic Verification

Cryptography can help prove properties such as:

- one credential was used only once;
- a vote was accepted;
- records were not modified after publication;
- a published result corresponds to the recorded votes;
- voter eligibility was established without revealing the voter's choice.

Zero-knowledge techniques may allow a system to prove eligibility or uniqueness without publishing personal identity information.

Cryptography protects records.

It does **not** prove that the original information was truthful.

Human institutions, independent observers, audits, and source verification therefore remain necessary.

---

# 15. Public Auditability

The protocol should publish sufficient information for independent parties to reproduce important calculations.

Possible participants include:

- citizens;
- journalists;
- researchers;
- auditors;
- courts;
- universities;
- civil society organizations;
- election observers;
- public institutions.

Voting software should be open source where legally and operationally appropriate.

Independent security audits should be required before deployment.

---

# 16. Threat Model

Clarus must assume that systems can fail.

Potential threats include:

- incorrect source data;
- compromised government systems;
- malicious administrators;
- software vulnerabilities;
- compromised voting machines;
- denial-of-service attacks;
- identity fraud;
- duplicate voting attempts;
- insider attacks;
- manipulation of physical ballots;
- coordinated misinformation;
- false or incomplete public records.

No single security mechanism is sufficient.

The protocol therefore uses multiple independent layers.

---

# 17. Blockchain

A public blockchain may be used as a tamper-evident publication layer.

The blockchain can help establish that:

- a record existed at a particular time;
- a published record was not silently modified;
- multiple independent participants retain copies of the record.

However:

> **A blockchain does not make false information true.**

If incorrect information is entered into the system, the blockchain can preserve the incorrect information perfectly.

Therefore the system requires independent source verification in addition to cryptographic integrity.

---

# 18. Privacy

Personal information should remain off-chain whenever possible.

The protocol should follow principles of:

- data minimization;
- purpose limitation;
- encryption;
- access control;
- separation of identity from political choice;
- secure deletion where legally required.

Public transparency must not become mass surveillance.

---

# 19. Governance

Clarus should remain politically neutral.

The protocol should not belong to:

- a political party;
- a government;
- a candidate;
- a private political campaign;
- or a single corporation.

Changes to the protocol should be publicly documented.

Important changes should undergo:

1. proposal;
2. public review;
3. technical review;
4. security review;
5. documented decision;
6. versioned release.

---

# 20. No Cryptocurrency Required

Clarus does not require a token.

There should be no mechanism where citizens can purchase additional voting power.

The purpose of the protocol is verification and transparency, not speculation.

The system should remain useful even if no cryptocurrency exists.

---

# 21. Country Implementations

Clarus is intended as a common protocol with country-specific implementations.

Each country may have different:

- constitutions;
- election laws;
- privacy laws;
- procurement systems;
- public accounting standards;
- government structures;
- identity systems.

The common principles remain:

**Transparency  
Auditability  
Privacy  
Independent verification  
One person, one vote  
Open standards  
No wealth-based political power**

The first implementation can be developed for Spain.

Other countries can adapt the protocol to their own legal and institutional systems.

---

# 22. Pilot

A responsible implementation should begin with a limited pilot.

The pilot should:

1. identify official public data sources;
2. normalize the data;
3. publish source references;
4. implement cryptographic integrity;
5. develop audit signals;
6. test independent verification;
7. conduct security testing;
8. test privacy protections;
9. conduct an extended public trial;
10. publish limitations and failures.

Voting infrastructure should not be used in a binding election until it has passed extensive independent testing and the applicable legal requirements.

---

# 23. What Clarus Does Not Claim

Clarus does not claim that:

- corruption can be made impossible;
- governments will always provide truthful data;
- algorithms can determine guilt;
- blockchain solves every security problem;
- technology can replace courts;
- technology can replace democratic institutions;
- elections can be made perfectly secure;
- or transparency alone solves every political problem.

The objective is narrower:

> **Make important public actions easier to verify independently.**

---

# 24. Conclusion

A government should not need to ask its citizens to trust that public resources were used correctly.

It should be possible to show the evidence.

A citizen should be able to follow public money.

A journalist should be able to verify a claim.

An auditor should be able to reproduce a calculation.

A voter should be able to verify that an election was conducted according to defined rules without revealing their private choice.

A public institution should be able to demonstrate what it did, what it spent, and what it delivered.

Clarus proposes an infrastructure for making this possible.

Not by replacing government.

Not by replacing democracy.

But by making the records of public power more transparent and independently verifiable.

> **Verify, do not trust.**
