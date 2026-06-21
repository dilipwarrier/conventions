# Requirements Documentation Conventions



## Purpose



This document defines shared conventions for requirements documentation

across the repository.



## Scope



These conventions apply to requirements documents for modules, tools,

and other documented system behaviors in this repository.



## Document Structure



Requirements documents shall use disciplined Markdown headings with the

following structure:



- `#` for the document title

- `##` for major sections such as `Overview` and `Functional

  Requirements`

- `###` for capability headings

- `####` for individual requirement identifiers



## Hierarchy



Requirements documents shall organize content using the following

hierarchy:



- **Capability**: a coherent area of externally visible system behavior

- **Functional Requirement**: a specific, testable statement of required

  behavior within a capability



## Requirement Identifier Format



Functional requirement identifiers shall use the following format:



`FR-<MODULE>-<CAPABILITY>-<NN>`



Where:



- `FR` identifies a functional requirement

- `<MODULE>` is the full stable module or domain name in uppercase, such

  as `CONTACTS`

- `<CAPABILITY>` is a stable uppercase capability code, such as `PARSE`,

  `DUE`, or `UPDATE`

- `<NN>` is a zero-padded ordinal within the capability, such as `01`



Examples:



- `FR-CONTACTS-PARSE-01`

- `FR-CONTACTS-DUE-12`



## Requirement Writing Conventions



Functional requirements shall follow these writing conventions:



- use normative language such as `shall`

- state behavior that is externally observable or testable

- remain implementation-neutral unless implementation detail is

  itself required behavior

- be atomic where practical

- include subordinate bullets or numbered lists only when enumerating

  values, fields, sort keys, or similar supporting details



## Stability and Maintenance



Requirement identifiers are intended to remain stable over time.



When updating a requirements document:



- add new requirements within the appropriate capability

- avoid global renumbering

- preserve existing identifiers when editing requirement wording

- remove obsolete requirements directly unless a separate retirement

  tracking process is introduced later



## Module Requirements Documents



A module-specific requirements document should:



- include a brief reference to this conventions document

- include an `Overview` section

- include a `Functional Requirements` section

- group requirements by capability

- express each functional requirement as a `####` heading followed by

  its normative text
