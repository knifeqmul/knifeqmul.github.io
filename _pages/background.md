---
title: "KNIFE - Background"
layout: gridlay
excerpt: "KNIFE -- Background."
sitemap: false
permalink: /background/
---



## Project

**KNIFE (Knowledge Discovery from Health Use Data)** is a Turing Institute funded project led by Dr William Marsh, with co-investigators Prof Norman Fenton, Prof Martin Neil, and Dr John Robson.

The increasing use and capability of Electronic Health Record (EHR) systems has made available large databases of patient records, linked across different health providers. These databases contain information about patients’ use of the different health services, treatments and prescriptions. The data, collected for clinical management or financial reporting, has many actual and potential uses including discovering causes, optimising health delivery, allocating resources and choosing treatment. However, there are both practical and technical challenges to overcome before these benefits can be achieved. The overall objective of the project is to lay the foundations for a transformative approach to patient-linked health data, making it accessible for both medical and data science researchers to fully exploit. We will achieve this by working with two groups who are custodians of data of this type in East London.

For full details see [here]({{ site.baseurl }}/downloads/Turing-proposal-marsh-4pages.pdf).


### Data origins
<figure class="center"> <img src="{{ site.url }}{{ site.baseurl }}/images/background/databases.png" style="width: 450px" align="middle">



### Database
Some tables in the database:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-kiyi{font-weight:bold;border-color:inherit;text-align:left}
.tg .tg-2dfk{font-weight:bold;background-color:#ecf4ff;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-xldj{border-color:inherit;text-align:left}
.tg .tg-fymr{font-weight:bold;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-2dfk">table</th>
    <th class="tg-2dfk">description</th>
  </tr>
  <tr>
    <td class="tg-kiyi">person</td>
    <td class="tg-xldj">links to personal information, including name, GP, address, and other information</td>
  </tr>
  <tr>
    <td class="tg-kiyi">person_prsnl_reltn</td>
    <td class="tg-xldj">patient's person relation, such as the primary care physician of the patient</td>
  </tr>
  <tr>
    <td class="tg-kiyi">order</td>
    <td class="tg-xldj">can pull orders, alerts, drugs administration and procedures</td>
  </tr>
  <tr>
    <td class="tg-kiyi">diagnosis and nomenclature</td>
    <td class="tg-xldj">keep various classifications like Snomed and ICD-10 can be tied to an encounter</td>
  </tr>
  <tr>
    <td class="tg-fymr">pathway</td>
    <td class="tg-0pky">store details about powerplans. A powerplan pre-prepared group of orders (such as <br>radiology, pathology, laboratory tests, medications, patient care etc) and <br>associated instructions for a specific condition, procedure or element of treatment<br>for faster electronic order entry</td>
  </tr>
  <tr>
    <td class="tg-fymr">clinical_event</td>
    <td class="tg-0pky">store patient encounter records per clinic, including information such as vital signs, <br>drugs administration time, and lab results</td>
  </tr>
</table>


Some notes about the **encounter** table.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;border-color:#bbb;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#bbb;color:#594F4F;background-color:#E0FFEB;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:#bbb;color:#493F3F;background-color:#9DE0AD;}
.tg .tg-v51t{font-weight:bold;background-color:#ecf4ff;border-color:#000000;text-align:center}
.tg .tg-q0fn{font-weight:bold;background-color:#ffffff;border-color:#000000;text-align:left}
.tg .tg-2pcy{background-color:#ffffff;border-color:#000000;text-align:left}
</style>
<table class="tg">
  <tr>
    <th class="tg-v51t">field name</th>
    <th class="tg-v51t">description of <span style="font-weight:700">table encounter</span></th>
  </tr>
  <tr>
    <td class="tg-q0fn">encntr_type_cd</td>
    <td class="tg-2pcy">Inpatient or outpatient encounter type</td>
  </tr>
  <tr>
    <td class="tg-q0fn">encntr_type_class_cd</td>
    <td class="tg-2pcy">classifies patients into more general groups such as emergency, recurring outpatient</td>
  </tr>
  <tr>
    <td class="tg-q0fn">reg_dt_tm</td>
    <td class="tg-2pcy">the registered or admitted date of the patient</td>
  </tr>
  <tr>
    <td class="tg-q0fn">active_ind</td>
    <td class="tg-2pcy">1 means the patient is active, 0 means the patiend has discharged</td>
  </tr>
</table>







### Glossary
**CCGs** - <a href='https://www.nhscc.org/ccgs/'>Clinical Commission Groups</a> commission most of the hospital and community NHS services in the local areas for which they are responsible. Commissioning involves deciding what services are needed for diverse local populations, and ensuring that they are provided.

**CRS** - Clinical Record System or Care Records Service?

**CSUs** - Commissioning Support Units provide CCGs with external support, specialist skills and knowledge to support them in their role as commissioners, including business intelligence services, clinical procurement services, business support services such as human resources, payroll, procurement of goods and services and some aspects of informatics.

**ELFT** - <a href='https://www.elft.nhs.uk/'>East London NHS Foundation Trust</a> (formerly known as East London and The City University Mental Health NHS Trust) was formed in April 2000. It provides mental health and community health services in East London and specialist services to a wider region.


**EMIS** - EMIS Health, formerly known as <a href='https://www.emishealth.com/'>Egton Medical Information Systems</a>, supplies electronic patient record systems and software used in primary care in England. It claims that more than half of GP practices across the UK use EMIS software.


**GP** - General practitioner, a family doctor who works from a local surgery to provide medical advice and treatment to patients registered on their list .

**HLP** - <a href='https://www.healthylondon.org/'>Healthy London Partnership</a> works with its partners to transform, connect and improve health and care so everyone in the capital can live healthier lives.

**RiO** - The electronic patient record system which holds information about referrals, appointments and clinical information.
