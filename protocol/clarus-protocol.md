# The Clarus Protocol

## A verifiable system for citizen voice and public money

**Version:** 0.2  
**Status:** Open proposal  
**Principle:** Verify, do not trust.

---

## 1. Purpose

The Clarus Protocol is an open framework for making public institutions more transparent, auditable, and better managed.

Clarus provides a common verification layer for:

- public money;
- public contracts;
- public projects and infrastructure;
- public compensation;
- government financial reporting;
- political and government promises;
- democratic processes;
- public audit signals.

Clarus does not replace constitutions, governments, legislatures, courts, electoral authorities, auditors, or existing legal systems.

Instead, it provides evidence and verification mechanisms that allow citizens, journalists, researchers, auditors, courts, legislators, and public institutions to independently examine public information.

The central principle is:

> **Verify, do not trust.**

The system should make it easier to determine what happened, who authorized it, what was paid, what was delivered, and what evidence supports the record.

---

## 2. Design Principles

### 2.1 Verify, do not trust

Important public claims should be independently verifiable whenever technically and legally possible.

Clarus should minimize dependence on a single institution, database, administrator, or trusted intermediary.

### 2.2 Open by default

Public information should be accessible in machine-readable and human-readable formats unless there is a legitimate legal, privacy, or security reason to restrict it.

### 2.3 Privacy by design

Transparency must not require exposing unnecessary personal information.

Personally identifiable information should be minimized, protected, or excluded from public records where appropriate.

### 2.4 Evidence before interpretation

Clarus records evidence and applies defined rules.

It should not turn a statistical anomaly into an accusation.

### 2.5 Signals are not conclusions

Automated systems may identify unusual patterns.

A risk signal means:

> "This deserves examination."

It does not mean:

> "Wrongdoing has been proven."

### 2.6 Independence

The system should minimize control by any single government, political party, company, administrator, or other interested party.

### 2.7 Legal compatibility

Country implementations must operate within the applicable constitution, laws, regulations, courts, electoral systems, privacy requirements, and administrative procedures.

### 2.8 No wealth-based political power

Clarus must never create a system where voting power depends on wealth, tokens, cryptocurrency holdings, reputation points, or financial contributions.

One eligible person must have one vote.

---

## 3. System Architecture

Clarus consists of several connected layers.

```text
                PUBLIC SOURCES
                     |
                     v
            +-------------------+
            |  DATA INGESTION   |
            +-------------------+
                     |
                     v
            +-------------------+
            | VALIDATION /      |
            | NORMALIZATION     |
            +-------------------+
                     |
                     v
            +-------------------+
            | CLARUS DATA MODEL |
            +-------------------+
                /     |      \
               /      |       \
              v       v        v
          MONEY    CONTRACTS   PEOPLE
              \      |        /
               \     |       /
                v    v      v
             AUDIT & VERIFICATION
                     |
          +----------+----------+
          |                     |
          v                     v
   PUBLIC EVIDENCE         RISK SIGNALS
          |                     |
          +----------+----------+
                     |
                     v
             PUBLIC INTERFACE
## 4. Source Data

Clarus should preferentially use authoritative public sources.

Examples include:

- government budgets;
- official accounting systems;
- procurement databases;
- contract registers;
- subsidy registers;
- parliamentary records;
- official salary records;
- public asset declarations where legally available;
- project completion records;
- official statistics;
- electoral registers and legally authorized voting records;
- court and audit records where publicly available.

Country implementations should maintain a public source registry.

Each source should contain, where available:

- source name;
- responsible institution;
- URL or access method;
- dataset identifier;
- publication date;
- update frequency;
- geographic scope;
- legal basis;
- data format;
- last successful ingestion;
- data quality information.

Clarus should never claim that it has complete national coverage unless completeness has actually been demonstrated.

---

## 5. Data Integrity

When data enters Clarus, the system should preserve evidence of the original source.

For each source artifact, Clarus may record:

- source identifier;
- retrieval timestamp;
- source version;
- cryptographic hash;
- transformation history;
- validation status.

A cryptographic hash can demonstrate that a stored copy has not been modified after ingestion.

However:

> A cryptographic hash proves the integrity of the stored data, not that the original information was true.

Truthfulness must therefore be addressed through source authority, cross-validation, audits, independent evidence, and legal procedures.

---

## 6. Public Money Protocol

Public money should be traceable through its lifecycle.

The core lifecycle is:

Budget
   ↓
Authorization
   ↓
Contract / Allocation
   ↓
Commitment
   ↓
Payment
   ↓
Delivery
   ↓
Verification
   ↓
Final Result

Where technically and legally possible, Clarus should connect these stages.

For a public project, the system should be able to answer:

- How much was authorized?
- Who authorized it?
- What was the purpose?
- Who received the contract?
- How much was contracted?
- How much was paid?
- When was it paid?
- What was delivered?
- Was the project completed?
- Was the final cost different from the original cost?
- Were modifications made?
- Who approved the modifications?
- What evidence confirms completion?

---

## 7. Government Financial Statement

Clarus should present public finances in a form that can be understood similarly to a transparent organization.

Where data permits, the system should expose:

### Revenue

- taxes;
- fees;
- social contributions;
- transfers;
- grants;
- other public income.

### Expenditure

- personnel;
- infrastructure;
- procurement;
- subsidies;
- social programs;
- transfers;
- debt servicing;
- international assistance;
- other expenditure.

### Assets

- public property;
- infrastructure;
- financial assets;
- other recorded assets.

### Liabilities

- public debt;
- obligations;
- guarantees;
- other liabilities.

### Cash flow

- money received;
- money paid;
- financing flows;
- changes in available cash.

### Fiscal position

Where applicable:

- deficit;
- surplus;
- debt;
- debt-to-revenue ratio;
- debt-to-GDP ratio;
- budget execution.

The system must clearly distinguish accounting concepts that are not directly comparable.

---

## 8. Public Contract Protocol

Every public contract should have a persistent identifier.

Where possible, the contract record should connect:

Contract
   |
   +-- Authority
   |
   +-- Tender
   |
   +-- Bidders
   |
   +-- Winner
   |
   +-- Contract value
   |
   +-- Amendments
   |
   +-- Payments
   |
   +-- Deliverables
   |
   +-- Completion
   |
   +-- Audit

The record should include, where legally available:

- contracting authority;
- procurement procedure;
- publication date;
- tender deadline;
- bidders;
- award decision;
- winning supplier;
- contract value;
- estimated value;
- contract duration;
- modifications;
- extensions;
- payments;
- completion status;
- responsible authority;
- associated project.

---

## 9. Supplier Identity

A supplier should have a persistent identifier within the country implementation.

Where legally available, the system may connect:

- legal entity;
- registration information;
- directors;
- beneficial ownership information;
- subsidiaries;
- parent entities;
- previous public contracts;
- contract values;
- sanctions;
- court decisions;
- relevant audit findings.

Sensitive personal information should not be exposed merely because a relationship exists in an internal dataset.

---

## 10. Public Project Protocol

Major public projects should be represented independently from individual contracts.

A project may contain:

- project identifier;
- geographic location;
- public authority;
- objective;
- original budget;
- revised budget;
- contracted amount;
- amount paid;
- expected completion date;
- actual completion date;
- contractors;
- subcontractors where legally available;
- modifications;
- completion evidence;
- audit records.

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
- public housing;
- energy infrastructure.

---

## 11. Comparable Cost Analysis

Clarus may compare similar public purchases and projects.

Comparisons should account for relevant differences such as:

- geographic location;
- scale;
- materials;
- technical specifications;
- labor costs;
- inflation;
- project complexity;
- contract duration;
- legal requirements.

The system should avoid simplistic comparisons such as:

> "Project A cost more than Project B, therefore something is wrong."

Instead it should produce an evidence-based signal such as:

> "The recorded unit cost is materially outside the comparison range for the selected comparable projects."

The methodology and comparison set must be visible.

---

## 12. Automated Audit Signals

Clarus may automatically generate signals from predefined rules.

Examples include:

- unusually high price;
- unusually high cost increase;
- repeated supplier wins;
- single-bid procurement;
- repeated contract modifications;
- contracts repeatedly extended;
- contracts split into smaller purchases;
- newly established supplier receiving unusually large contracts;
- payments made before expected milestones;
- payment without corresponding completion evidence;
- supplier concentration;
- unusual geographic or organizational patterns;
- inconsistent dates;
- inconsistent financial values.

Each signal should contain:

Signal ID  
Rule ID  
Affected record  
Source data  
Calculation  
Threshold  
Comparison set  
Timestamp  
Confidence / uncertainty  
Status  
Response

---

## 13. Risk Signal Lifecycle

A signal should follow this lifecycle:

Detected
   ↓
Published
   ↓
Reviewed
   ↓
Response / Evidence
   ↓
Resolved / Unresolved
   ↓
Archived

Possible statuses include:

- open;
- under review;
- explained;
- corrected;
- unresolved;
- referred to competent authority;
- closed.

A signal must not automatically become a finding of misconduct.

---

## 14. Right of Reply

When a public institution, official, company, or other affected party is associated with a public audit signal, the applicable legal implementation should provide an opportunity to submit evidence or clarification where appropriate.

Responses should be recorded with:

- respondent;
- date;
- evidence submitted;
- response status;
- reviewer;
- final disposition.

The original record should not be silently deleted.

Corrections should create an auditable history.

---

## 15. Public Compensation Protocol

Clarus should make public compensation understandable and auditable.

Where legally available, records may include:

- position;
- institution;
- base salary;
- allowances;
- bonuses;
- expenses;
- benefits;
- public compensation components;
- applicable legal framework.

For public officials, compensation should be distinguishable from legitimate reimbursement of public expenses.

The system should not expose unnecessary private information.

---

## 16. Public Pay Ladder

A country implementation may define a public compensation framework based on objective parameters.

One possible model is a multiple of the applicable minimum wage.

For example:

Head of government       ≤ 50 × minimum wage  
Senior national office  = defined fraction  
Other public offices     = defined bands

These values are illustrative and must not be treated as universal Clarus requirements.

A country may choose another legally established compensation methodology.

The protocol requirement is that the methodology be:

- public;
- objective;
- consistently applied;
- legally defined;
- auditable.

---

## 17. Government Promise Protocol

Public promises and commitments may be recorded as structured claims.

A promise record may contain:

- speaker;
- position;
- date;
- source;
- exact statement;
- policy area;
- intended outcome;
- expected timeframe;
- legal or institutional dependency;
- implementation status.

Possible statuses include:

- proposed;
- adopted;
- funded;
- in progress;
- delayed;
- completed;
- partially completed;
- cancelled;
- reversed;
- superseded.

A change in policy should not automatically be classified as dishonesty.

The system should record the evidence and explain the status.

---

## 18. Performance Evidence

Where measurable outcomes exist, Clarus may connect promises to evidence.

Example:

Promise
   ↓
Policy / Law
   ↓
Budget
   ↓
Implementation
   ↓
Measured outcome

The system should distinguish:

- what was promised;
- what was legally enacted;
- what was funded;
- what was implemented;
- what measurable result occurred.

This prevents a political statement from being treated as equivalent to a completed policy.

---

## 19. Identity Protocol

Clarus voting systems must establish eligibility without revealing the voter's choice.

The identity layer should establish:

1. the person is eligible;
2. the person has not already voted;
3. the person receives one voting credential;
4. the credential cannot reveal the person's vote.

Where technically appropriate, anonymous credentials or zero-knowledge proofs may be used.

The identity system and ballot system must be cryptographically and operationally separated.

---

## 20. Voting Protocol

Clarus supports legally authorized democratic voting systems that preserve:

- eligibility;
- one person, one vote;
- ballot secrecy;
- auditability;
- accessibility;
- independent verification.

A reference in-person model is:

IDENTITY VERIFICATION
        ↓
VOTER REGISTER
        ↓
BALLOT / CREDENTIAL ISSUED
        ↓
PRIVATE VOTING
        ↓
DIGITAL VOTE
        +
ANONYMOUS PAPER BALLOT
        ↓
COUNT
        ↓
PUBLIC AUDIT

The exact implementation must be adapted to the country's electoral law.

---

## 21. One-Day Voting Window

A Clarus-compatible election may use a defined voting window.

A reference design is:

> One internationally coordinated 24-hour voting period.

Authorized polling locations may operate in:

- the voter's country;
- diplomatic facilities;
- other legally authorized international polling locations.

The voting period and locations must be publicly defined before the election.

Exceptions for people who cannot reasonably access an authorized polling location must be determined by the applicable electoral authority and law.

Remote voting should not be introduced merely for convenience where it creates unacceptable security or coercion risks.

---

## 22. Manual Voter Register

In a reference in-person implementation, the voter may:

1. present an approved identity document;
2. be verified as eligible;
3. sign or otherwise authenticate the official voter record;
4. receive a voting credential or ballot authorization;
5. vote privately.

The voter register must never contain information linking the voter's identity to their selected candidate or option.

---

## 23. Private Digital Vote

The electronic voting system may use cryptographic techniques to prove:

- the voter was eligible;
- the voter received a valid voting credential;
- the credential was used only once;
- the vote was accepted;
- the final tally corresponds to valid votes.

Where zero-knowledge techniques are used, they should prove validity without revealing the voter's selection.

No public blockchain record should contain:

- the voter's identity;
- the voter's signature;
- passport number;
- national identification number;
- personal voting history;
- any identifier that can directly link a person to a vote.

---

## 24. Printed Ballot

A reference implementation may produce a physical paper record after the digital selection.

The printed ballot should show only the voter's choice or the legally required ballot information.

It must not contain:

- name;
- identity number;
- signature;
- voter credential;
- personal identifier;
- traceable serial number;
- QR code linking the ballot to the voter.

The voter should verify the paper record and deposit it into a secure ballot box.

The physical ballot provides an independent audit trail.

---

## 25. Three-Way Reconciliation

A core Clarus voting principle is reconciliation between three independent records:

### A. Eligibility / ballot issuance

How many verified eligible voters received authorization to vote?

### B. Anonymous physical ballots

How many physical ballots were deposited?

### C. Digital votes

How many valid electronic votes were accepted?

The system should reconcile these quantities under legally defined procedures.

Conceptually:

Verified voters
      |
      v
Ballot authorization
      |
      +----------+
      |          |
      v          v
 Digital      Paper
  vote        ballot
      |          |
      +-----+----+
            |
            v
        Reconciliation
            |
            v
        Final result

Any unexplained discrepancy must trigger an audit process.

---

## 26. Paper Audit Independence

The electronic result must not be considered automatically authoritative merely because it was generated by software.

The physical ballot record provides an independent verification mechanism.

Election law should define:

- when recounts occur;
- how random audits are selected;
- how discrepancies are resolved;
- who supervises recounts;
- how observers participate;
- what evidence is preserved.

---

## 27. Public Voting Verification

After an election, Clarus may publish cryptographic evidence demonstrating that:

- valid voting credentials were accepted;
- duplicate voting was prevented;
- votes were counted according to the protocol;
- the published result corresponds to the accepted ballots;
- the anonymous ballot record was preserved.

The verification process must not allow anyone to determine how an individual voted.

---

## 28. Blockchain Layer

Blockchain or another append-only distributed ledger may be used where it provides meaningful value.

Possible uses include recording:

- hashes of official documents;
- timestamps;
- dataset versions;
- audit events;
- cryptographic proofs;
- election verification commitments.

The ledger should not be used merely because it is fashionable.

A blockchain does not guarantee that an input is truthful.

Therefore:

Source truth
    ≠
Cryptographic integrity

Both are necessary.

---

## 29. Personal Data

Personal data should remain off the public ledger wherever possible.

The system should use:

- data minimization;
- encryption;
- access control;
- pseudonymization;
- anonymous credentials;
- zero-knowledge proofs;
- legally defined retention periods.

Public transparency must not become mass surveillance.

---

## 30. Sensitive Public Information

Certain information may require restricted access for legitimate reasons.

Examples may include:

- security-sensitive infrastructure;
- protected witnesses;
- intelligence personnel;
- operational military information;
- personal addresses;
- information whose publication creates a demonstrated safety risk.

Restrictions must have a legal basis.

A restriction should not simply be applied because disclosure is politically inconvenient.

Where possible, the system should publish a redacted explanation of why information is unavailable.

---

## 31. Public Access

Clarus should provide both:

### Human-readable access

Dashboards, charts, explanations, documents, timelines and searchable records.

### Machine-readable access

APIs, structured datasets, hashes, metadata and downloadable records.

The same underlying evidence should support both interfaces.

---

## 32. Data Provenance

Every important public record should have traceable provenance.

A user should be able to determine:

Where did this information come from?
        ↓
When was it obtained?
        ↓
Was it transformed?
        ↓
What transformations occurred?
        ↓
What calculations were applied?
        ↓
What evidence supports the result?

This is essential for independent verification.

---

## 33. Corrections

Clarus should never silently rewrite historical records.

If information is corrected:

Original record
      ↓
Correction
      ↓
Reason
      ↓
New record

The system should preserve the audit history.

This allows observers to distinguish:

- original publication;
- error;
- correction;
- later information.

---

## 34. Governance

The protocol should be governed through transparent, documented rules.

Governance should address:

- protocol changes;
- software releases;
- security vulnerabilities;
- data-source disputes;
- rule changes;
- country implementations;
- emergency procedures.

No single person should have unilateral control over the global protocol.

---

## 35. Protocol Changes

Changes should be:

1. proposed publicly;
2. documented;
3. technically reviewed;
4. security reviewed where appropriate;
5. open for public comment;
6. versioned;
7. approved according to the governance rules;
8. published with a changelog.

Breaking changes require a new protocol version.

---

## 36. Country Implementations

Clarus is designed as a global protocol with country-specific implementations.

The global layer defines common principles.

Each country defines:

- legal identity requirements;
- public data sources;
- procurement rules;
- accounting standards;
- electoral law;
- privacy requirements;
- public compensation rules;
- institutions;
- language;
- implementation details.

For example:

Clarus Protocol
       |
       +------ Spain
       |
       +------ France
       |
       +------ Germany
       |
       +------ United States
       |
       +------ Other countries

A country implementation must not change the fundamental principles of:

- auditability;
- privacy;
- one-person-one-vote;
- evidence preservation;
- source transparency.

---

## 37. Interoperability

Country implementations should use common identifiers and standards where possible.

Examples include:

- Open Contracting Data Standard;
- common geographic identifiers;
- internationally recognized organization identifiers;
- standardized timestamps;
- standardized currencies;
- machine-readable metadata.

Interoperability allows cross-country research without requiring countries to use identical legal systems.

---

## 38. Audit Independence

Clarus should support multiple independent verification parties.

Possible participants include:

- national audit institutions;
- courts;
- universities;
- journalists;
- civil-society organizations;
- independent auditors;
- researchers;
- citizens;
- international observers.

No participant should automatically be considered correct solely because of institutional status.

Evidence should remain inspectable.

---

## 39. Threat Model

Clarus must consider attacks and failures including:

### Data manipulation

A source publishes incorrect information.

### Data omission

Important information is never published.

### Database manipulation

Records are altered after ingestion.

### Software bugs

The system calculates an incorrect result.

### Identity fraud

Someone attempts to obtain multiple voting credentials.

### Vote manipulation

An attacker attempts to alter electronic votes.

### Ballot manipulation

Physical ballots are lost, destroyed, substituted, or incorrectly counted.

### Denial of service

Citizens cannot access the system.

### Insider attacks

Authorized administrators misuse privileges.

### Political capture

A government, party, company, or other actor attempts to control the system.

### Privacy attacks

An attacker attempts to identify citizens or infer their votes.

Clarus cannot eliminate every threat.

The objective is to make attacks:

- harder;
- more detectable;
- independently auditable;
- recoverable.

---

## 40. Security Model

Critical components should use:

- multi-party authorization;
- independent infrastructure;
- cryptographic signing;
- immutable audit logs;
- secure backups;
- open-source software;
- reproducible builds where practical;
- independent security audits;
- penetration testing;
- incident-response procedures.

No single administrator should be able to silently alter critical historical records.

---

## 41. Software Transparency

Core Clarus software should be open source.

The public should be able to inspect:

- source code;
- protocol specifications;
- cryptographic methods;
- audit rules;
- data schemas;
- software versions;
- security reports;
- material protocol changes.

Open source does not automatically mean secure.

Independent review remains necessary.

---

## 42. Automated Decision Limits

Clarus should not automatically:

- accuse a person of corruption;
- declare a company fraudulent;
- determine criminal responsibility;
- remove an elected official;
- determine legal guilt;
- determine election legitimacy without the legally authorized process.

Automated systems may identify evidence requiring human or institutional review.

---

## 43. Citizen Review

Citizens should be able to:

- inspect public records;
- follow government spending;
- examine contracts;
- compare projects;
- review public compensation;
- examine promises and outcomes;
- inspect audit signals;
- submit evidence;
- request clarification;
- follow corrections.

The purpose is to reduce the information gap between institutions and the public.

---

## 44. Democratic Accountability

Clarus does not itself remove elected officials.

Where a country's constitution or law provides mechanisms such as:

- recall elections;
- referendums;
- impeachment;
- votes of no confidence;
- judicial procedures;

Clarus may provide the evidence and verification infrastructure needed to support those processes.

The authority to remove an official remains with the legally authorized institution or electorate.

---

## 45. Funding

Clarus should avoid financial structures that create conflicts of interest.

Possible funding models may include:

- public-interest grants;
- transparent donations;
- philanthropic funding;
- institutional partnerships;
- research funding.

All significant funding should be publicly disclosed.

Funding must not grant control over:

- audit results;
- data;
- voting;
- protocol rules;
- investigations.

---

## 46. No Voting Token

Clarus does not require a cryptocurrency.

There should be no:

1 token = 1 vote

and no:

More money = more political power

Voting rights must come from legal democratic eligibility, not ownership of a financial asset.

---

## 47. Economic Neutrality

Clarus is not designed to favor:

- public ownership;
- private ownership;
- higher taxes;
- lower taxes;
- larger government;
- smaller government;
- any political party;
- any political ideology.

The protocol's function is to make decisions and their consequences more observable and verifiable.

---

## 48. Implementation Requirements

Before a country deploys a production Clarus implementation, it should demonstrate:

1. legal compatibility;
2. data-source mapping;
3. security testing;
4. privacy assessment;
5. independent audit;
6. public documentation;
7. disaster recovery;
8. governance procedures;
9. source-data validation;
10. user testing;
11. accessibility testing;
12. election testing where voting is included.

Voting systems should undergo extensive testing before being used in a binding election.

---

## 49. Pilot Deployment

Implementation should begin with a limited pilot.

A possible sequence is:

Phase 1
Public data inventory
        ↓
Phase 2
Data ingestion
        ↓
Phase 3
Public contracts
        ↓
Phase 4
Public money
        ↓
Phase 5
Compensation
        ↓
Phase 6
Promise tracking
        ↓
Phase 7
Audit signals
        ↓
Phase 8
Voting verification prototype
        ↓
Phase 9
Independent security audit
        ↓
Phase 10
Public pilot
        ↓
Production implementation

The voting system should not be the first component deployed at national scale.

---

## 50. Spain Reference Implementation

The first country implementation may be Spain.

The Spain implementation should connect, where legally and technically possible, to official sources covering:

- national budgets;
- public expenditure;
- public contracts;
- public employees;
- senior officials;
- parliamentary information;
- subsidies;
- public projects;
- transparency information;
- electoral information.

The Spain implementation should preserve Spanish legal requirements while following the common Clarus architecture.

Spain-specific implementation details belong in:

`countries/spain/`

They should not be hard-coded into the global protocol.

---

## 51. Global vs Country Layer

The distinction is:

### Global Clarus Protocol

Defines:

- principles;
- architecture;
- data concepts;
- audit philosophy;
- privacy principles;
- cryptographic requirements;
- voting principles;
- interoperability;
- governance principles.

### Country Implementation

Defines:

- legal rules;
- institutions;
- official sources;
- local identifiers;
- local accounting;
- electoral procedures;
- privacy law;
- public compensation rules;
- procurement rules.

This separation allows Clarus to operate internationally without pretending that every country's institutions are identical.

---

## 52. Core Data Objects

The minimum conceptual objects are:

Person
Organization
PublicInstitution
OfficialPosition
Compensation
Budget
Transaction
Contract
Tender
Supplier
Project
Payment
Deliverable
Promise
Policy
AuditEvent
RiskSignal
Election
VoterCredential
Ballot
Vote
Source
Document

Detailed schemas are defined in:

`protocol/data-model.md`

---

## 53. Minimum Audit Trail

For every critical event, Clarus should preserve:

Who / which institution acted  
What happened  
When it happened  
What source proves it  
What data was used  
What transformation occurred  
What rule was applied  
What result was produced  
What correction occurred later

---

## 54. Core Invariant

The central system invariant is:

> **A public claim should be traceable to evidence.**

And:

> **A system-generated conclusion should be traceable to a documented rule applied to identifiable evidence.**

This allows a third party to reproduce the reasoning.

---

## 55. Reproducibility

Whenever practical, an independent researcher should be able to reproduce an audit result from:

- the published source data;
- the documented transformation;
- the documented rule;
- the relevant version of the software.

If a result cannot be reproduced, the limitation should be documented.

---

## 56. Versioning

Every protocol, dataset, rule, and software release should have a version.

Example:

Protocol: 0.2  
Data model: 0.1  
Rules: 0.1  
Spain implementation: 0.1  
Software: 0.1.x

Historical results should remain associated with the version that generated them.

---

## 57. What Clarus Does Not Claim

Clarus does not claim that:

- corruption can be made impossible;
- blockchain makes information truthful;
- software cannot fail;
- every anomaly indicates wrongdoing;
- every public decision can be reduced to a numerical score;
- technology can replace courts;
- technology can replace democratic institutions;
- elections can be made risk-free;
- transparency eliminates political disagreement.

Clarus instead seeks to make evidence easier to access, preserve, compare, and verify.

---

## 58. Fundamental Principle

The system can be summarized as:

PUBLIC DATA
     ↓
VERIFIED SOURCES
     ↓
PRESERVED EVIDENCE
     ↓
TRANSPARENT RULES
     ↓
REPRODUCIBLE ANALYSIS
     ↓
PUBLIC VERIFICATION
     ↓
LEGAL / DEMOCRATIC ACTION

The protocol should never reverse this order by starting with a conclusion and searching for evidence afterward.

---

## 59. Conclusion

Clarus is a public verification protocol.

Its purpose is not to decide what citizens should believe.

Its purpose is to make it easier for citizens to determine:

- where public money came from;
- where it went;
- what was purchased;
- who received it;
- what was delivered;
- what was promised;
- what happened afterward;
- how public institutions performed;
- how democratic processes were conducted;
- and what evidence supports each claim.

The system is built around one principle:

> **Verify, do not trust.**

Clarus should make public institutions easier to understand, public resources easier to audit, and democratic processes easier to verify.

It should provide evidence without becoming the authority that decides what the evidence means.

---

# Appendix A — Reference Architecture

```text
                    CLARUS PROTOCOL
                           |
        +------------------+------------------+
        |                  |                  |
        v                  v                  v
   PUBLIC MONEY       PUBLIC CONTRACTS     PUBLIC PEOPLE
        |                  |                  |
        +------------------+------------------+
                           |
                           v
                 GOVERNMENT FINANCES
                           |
                           v
                  PROMISE / PERFORMANCE
                           |
                           v
                    AUDIT ENGINE
                           |
              +------------+------------+
              |                         |
              v                         v
       PUBLIC EVIDENCE             RISK SIGNALS
              |                         |
              +------------+------------+
                           |
                           v
                  PUBLIC VERIFICATION
                           |
              +------------+------------+
              |                         |
              v                         v
        CITIZEN REVIEW             LEGAL PROCESS


                    DEMOCRATIC LAYER
                           |
                    IDENTITY / ELIGIBILITY
                           |
                    ANONYMOUS CREDENTIAL
                           |
                  +--------+--------+
                  |                 |
                  v                 v
             DIGITAL VOTE      PAPER BALLOT
                  |                 |
                  +--------+--------+
                           |
                    RECONCILIATION
                           |
                           v
                     PUBLIC AUDIT
