---
title: "KNIFE - Code"
layout: textlay
excerpt: "KNIFE - Code"
sitemap: false
permalink: /code/
---

## Code

some notes about the **encounter** table.


| field name           	| description                                                                          	|
|----------------------	|--------------------------------------------------------------------------------------	|
| encntr_type_cd       	| Inpatient or outpatient encounter type                                               	|
| encntr_type_class_cd 	| classifies patients into more general groups such as emergency, recurring outpatient 	|
| reg_dt_tm            	| the registered or admitted date of the patient                                       	|
| active_ind           	| 1 means the patient is active, 0 means the patiend has discharged                    	|

some notes about the **encounter** table.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-xldj{border-color:inherit;text-align:left}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-c3ow">table</th>
    <th class="tg-c3ow">description</th>
  </tr>
  <tr>
    <td class="tg-xldj">person</td>
    <td class="tg-xldj">links to personal information, including name, GP, address, and other information</td>
  </tr>
  <tr>
    <td class="tg-xldj">person_prsnl_reltn</td>
    <td class="tg-xldj">patient's person relation, such as the primary care physician of the patient</td>
  </tr>
  <tr>
    <td class="tg-xldj">order</td>
    <td class="tg-xldj">can pull orders, alerts, drugs administration and procedures</td>
  </tr>
  <tr>
    <td class="tg-xldj">diagnosis and nomenclature</td>
    <td class="tg-xldj">keep various classifications like Snomed and ICD-10 can be tied to an encounter</td>
  </tr>
  <tr>
    <td class="tg-0pky">pathway</td>
    <td class="tg-0pky">store details about powerplans. A powerplan pre-prepared group of orders (such as <br>radiology, pathology, laboratory tests, medications, patient care etc) and <br>associated instructions for a specific condition, procedure or element of treatment<br>for faster electronic order entry</td>
  </tr>
  <tr>
    <td class="tg-0pky">clinical_event</td>
    <td class="tg-0pky">store patient encounter records per clinic, including information such as vital signs, <br>drugs administration time, and lab results</td>
  </tr>
</table>
