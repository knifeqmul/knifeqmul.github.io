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


<br>

##### **Coding**
Different coding systems are in use through the HES datasets. Diagnoses in the Hospital admissions records (aka Admitted Patient Care, APC) and Outpatient Records (OP) datasets are coded using the International Classification of Disease (ICD) clinical classification system. Entries up until 1995 were coded using ICD 9 and subsequent entries with ICD 10. 
Establishing data interoperability between information coded to ICD 9 and ICD 10 can be challenging. Operative procedures are coded using the Office of Population Censuses and Survey’s (OPCS) version 4 clinical classification. Both classification systems are updated periodically to accommodate new conditions. NHS coding and classification standards – and cross-mapping reference files -
are managed by the ‘Technology Reference data Update Distribution’ (TRUD) unit, that is part of NHS Digital40. 

Within the A&E dataset, bespoke classifications are used within the AEPATGROUP (recording the reason for an A&E attendance) and DIAG2_NN fields (The A&E diagnosis comprises a six-character code made up of: diagnosis condition, sub-analysis, anatomical area and anatomical side).

Currently the NHS is moving to adopt the SNOMED CT nomenclature, and separately the WHO is working with SNOMED CT regarding the development of the ICD 11 standard.






<br>

##### **Data Quality**

Results of the Audit Commission’s 2009 national clinical coding audit in selected specialties in a large NHS Trust.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-zlqz{font-weight:bold;background-color:#c0c0c0;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-3r9o{font-weight:bold;background-color:#c0c0c0;border-color:inherit;text-align:center}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{font-weight:bold;border-color:inherit;text-align:center;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-3r9o">Area audited</th>
    <th class="tg-zlqz">Primary<br>Diagnoses<br>Incorrect<br>(%)</th>
    <th class="tg-zlqz">Secondary<br>Diagnoses<br>Incorrect<br>(%)</th>
    <th class="tg-zlqz">Primary<br>Procedures<br>Incorrect<br>(%)</th>
    <th class="tg-zlqz">Secondary<br>Procedures<br>Incorrect<br>(%)</th>
  </tr>
  <tr>
    <td class="tg-c3ow">Theme – 110: Trauma &amp; Orthopaedics</td>
    <td class="tg-c3ow">20</td>
    <td class="tg-c3ow">24.9</td>
    <td class="tg-c3ow">19.1</td>
    <td class="tg-c3ow">12.4</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Speciality – 502: Gynaecology</td>
    <td class="tg-c3ow">8</td>
    <td class="tg-c3ow">19.7</td>
    <td class="tg-c3ow">12.4</td>
    <td class="tg-c3ow">12.5</td>
  </tr>
  <tr>
    <td class="tg-c3ow">HRG Chapter – L: Urinary Tract <br>and Male Reproductive System</td>
    <td class="tg-c3ow">12.9</td>
    <td class="tg-c3ow">25.4</td>
    <td class="tg-c3ow">14.3</td>
    <td class="tg-c3ow">35.5</td>
  </tr>
  <tr>
    <td class="tg-c3ow">HRG – F36: Large Intestinal<br>Disorders &gt;69</td>
    <td class="tg-c3ow">3.3</td>
    <td class="tg-c3ow">28.3</td>
    <td class="tg-c3ow">27.3</td>
    <td class="tg-c3ow">7.1</td>
  </tr>
  <tr>
    <td class="tg-7btt">Overall</td>
    <td class="tg-7btt">12.7</td>
    <td class="tg-7btt">24.4</td>
    <td class="tg-7btt">15.9</td>
    <td class="tg-7btt">15.3</td>
  </tr>
</table>

<br>


