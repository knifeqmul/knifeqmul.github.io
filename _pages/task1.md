---
title: "KNIFE - Task1"
layout: textlay
excerpt: "KNIFE - Task1"
sitemap: false
permalink: /task1/
---


#### **Task 1: Data Description at Several Levels of Abstraction.**

*  Create a simplified model of the data generation process, covering the organisations involved, using a mix of text and diagrams.
*  Create a semantic schema, using web ontology techniques or related techniques. We will also investigate the use and role of the medical ontologies used to tag data (primarily SNOMED).
*  Investigate the mapping between the semantic schema and the storage schema, its use for data access and the potential for automating its construction.

This task will result in a description of the data that can be shared with potential collaborators. A complete data dictionary may not be necessary if the same concepts recur in different parts of the data.


##### Coding
Different coding systems are in use through the HES datasets. Diagnoses in the Hospital admissions records (aka Admitted Patient Care, APC) and Outpatient Records (OP) datasets are coded using the International Classification of Disease (ICD) clinical classification system. Entries up until 1995 were coded using ICD 9 and subsequent entries with ICD 10. 
Establishing data interoperability between information coded to ICD 9 and ICD 10 can be challenging. Operative procedures are coded using the Office of Population Censuses and Survey’s (OPCS) version 4 clinical classification. Both classification systems are updated periodically to accommodate new conditions. NHS coding and classification standards – and cross-mapping reference files -
are managed by the ‘Technology Reference data Update Distribution’ (TRUD) unit, that is part of NHS Digital40. 

Within the A&E dataset, bespoke classifications are used within the AEPATGROUP (recording the reason for an A&E attendance) and DIAG2_NN fields (The A&E diagnosis comprises a six-character code made up of: diagnosis condition, sub-analysis, anatomical area and anatomical side).

Currently the NHS is moving to adopt the SNOMED CT nomenclature, and separately the WHO is working with SNOMED CT regarding the development of the ICD 11 standard.