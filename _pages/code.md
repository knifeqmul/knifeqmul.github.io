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

| table                      	| description                                                                                                                                                                                                                                                                          	|
|----------------------------	|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| person                     	| links to personal information, including name, GP, address, and other information                                                                                                                                                                                                    	|
| person_prsnl_reltn         	| patient's person relation, such as the primary care physician of the patient                                                                                                                                                                                                         	|
| order                      	| can pull orders, alerts, drugs administration and procedures                                                                                                                                                                                                                         	|
| diagnosis and nomenclature 	| keep various classifications like Snomed and ICD-10 can be tied to an encounter                                                                                                                                                                                                      	|
| pathway                    	| store details about powerplans. A powerplan pre-prepared group of orders (such as  radiology, pathology, laboratory tests, medications, patient care etc) and  associated instructions for a specific condition, procedure or element of treatment for faster electronic order entry 	|
| clinical_event             	| store patient encounter records per clinic, including information such as vital signs,  drugs administration time, and lab results                                                                                                                                                   	|
