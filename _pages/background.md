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
.tg .tg-qtf5{border-color:#000000;text-align:left}
.tg .tg-v51t{font-weight:bold;background-color:#ecf4ff;border-color:#000000;text-align:center}
.tg .tg-v47y{font-weight:bold;border-color:#000000;text-align:left}
.tg .tg-mcqj{font-weight:bold;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-v51t">table</th>
    <th class="tg-v51t">description</th>
  </tr>
  <tr>
    <td class="tg-v47y">person</td>
    <td class="tg-qtf5">links to personal information, including name, GP, address, and other information</td>
  </tr>
  <tr>
    <td class="tg-v47y">person_prsnl_reltn</td>
    <td class="tg-qtf5">patient's person relation, such as the primary care physician of the patient</td>
  </tr>
  <tr>
    <td class="tg-v47y">order</td>
    <td class="tg-qtf5">can pull orders, alerts, drugs administration and procedures</td>
  </tr>
  <tr>
    <td class="tg-v47y">diagnosis and nomenclature</td>
    <td class="tg-qtf5">keep various classifications like ICD-10 can be tied to an encounter</td>
  </tr>
  <tr>
    <td class="tg-mcqj">pathway</td>
    <td class="tg-73oq">store details about powerplans. A powerplan pre-prepared group of orders (such as radiology, pathology, laboratory tests, medications, patient care etc) and associated instructions for a specific condition, procedure or element of treatmentfor faster electronic order entry</td>
  </tr>
  <tr>
    <td class="tg-mcqj">clinical_event</td>
    <td class="tg-73oq">store patient encounter records per clinic, including information such as vital signs, drugs administration time, and lab results</td>
  </tr>
</table>

<br>
Some notes about the **encounter** table.
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-qtf5{border-color:#000000;text-align:left}
.tg .tg-v51t{font-weight:bold;background-color:#ecf4ff;border-color:#000000;text-align:center}
.tg .tg-v47y{font-weight:bold;border-color:#000000;text-align:left}
</style>
<table class="tg">
  <tr>
    <th class="tg-v51t">field name</th>
    <th class="tg-v51t">description of table encounter</th>
  </tr>
  <tr>
    <td class="tg-v47y">encntr_type_cd</td>
    <td class="tg-qtf5">Inpatient or outpatient encounter type</td>
  </tr>
  <tr>
    <td class="tg-v47y">encntr_type_class_cd</td>
    <td class="tg-qtf5">classifies patients into more general groups such as emergency, recurring outpatient</td>
  </tr>
  <tr>
    <td class="tg-v47y">reg_dt_tm</td>
    <td class="tg-qtf5">the registered or admitted date of the patient</td>
  </tr>
  <tr>
    <td class="tg-v47y">active_ind</td>
    <td class="tg-qtf5">1 means the patient is active, 0 means the patiend has discharged</td>
  </tr>
</table>



### Classification schema

Classification schema when recording relevant medical information and events. These codes can vary between institutions, and maintained by terminology like Systemized Nomenclature of Medicine - Clinical Terms (SNOMED CT) or READ codes (see <a href="http://www.gp-training.net/it/synergy_archive/synergy/readcode.htm">[here]</a>). The following table is from [1]:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-2dfk{font-weight:bold;background-color:#ecf4ff;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-ohmh{font-weight:bold;background-color:#ecf4ff;border-color:inherit;text-align:center}
.tg .tg-xldj{border-color:inherit;text-align:left}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-ohmh">Schema </th>
    <th class="tg-ohmh">Number of Codes</th>
    <th class="tg-2dfk">Examples</th>
  </tr>
  <tr>
    <td class="tg-xldj">ICD-10(Diagnosis)</td>
    <td class="tg-xldj">68,000</td>
    <td class="tg-0pky">- J9600: Acute respiratory failure<br>- I509: Heart failure<br>- I5020: Systolic heart failure</td>
  </tr>
  <tr>
    <td class="tg-xldj">CPT(Procedures)</td>
    <td class="tg-xldj">9,641</td>
    <td class="tg-0pky">- 72146: MRI Thoracic Spine<br>- 67810: Eyelid skin biopsy<br>- 19301: Partial mastectomy<br></td>
  </tr>
  <tr>
    <td class="tg-xldj">LOINC(Laboratory)</td>
    <td class="tg-xldj">80,868</td>
    <td class="tg-0pky">- 4024-6: Salicylate, Serum<br>- 56478-1: Ethanol, Blood<br><br>- 3414-0: Buprenorphine Screen<br></td>
  </tr>
  <tr>
    <td class="tg-xldj">RxNorm(Medications)</td>
    <td class="tg-xldj">116,075</td>
    <td class="tg-0pky">- 161: Acetaminophen<br>- 7052: Morphine<br>- 1819: Buprenorphine</td>
  </tr>
  
</table>


[1] Shickel, B., Tighe, P. J., Bihorac, A., & Rashidi, P. (2018). Deep EHR: a survey of recent advances in deep learning techniques for electronic health record (EHR) analysis. IEEE journal of biomedical and health informatics, 22(5), 1589-1604.

### Terminology

SNOMED CT and READ codes are terminology designed for use in electronic health records. A more detailed introduction of Read codes see [here]({{ site.baseurl }}/downloads/readcodehier.pdf), a list of codes can be found [here]({{ site.baseurl }}/downloads/acc6343-read-codes.xls).


#### 1.Read Code - Process of Care
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-uril{color:#000000;border-color:#000000;text-align:left}
.tg .tg-h8n2{font-weight:bold;color:#000000;border-color:#000000;text-align:left}
.tg .tg-4yk5{font-weight:bold;background-color:#ecf4ff;color:#000000;border-color:#000000;text-align:center}
.tg .tg-8fiv{font-weight:bold;color:#000000;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-pjk6{color:#000000;border-color:#000000;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-4yk5" colspan="4">Process of Care</th>
  </tr>
  <tr>
    <td class="tg-h8n2">0<br></td>
    <td class="tg-uril">Occupations</td>
    <td class="tg-h8n2">5</td>
    <td class="tg-uril">Radiology</td>
  </tr>
  <tr>
    <td class="tg-h8n2">1</td>
    <td class="tg-uril">History and Symptoms</td>
    <td class="tg-h8n2">6</td>
    <td class="tg-uril">Preventative Procedures</td>
  </tr>
  <tr>
    <td class="tg-h8n2">2</td>
    <td class="tg-uril">Examinations and Signs</td>
    <td class="tg-h8n2">7</td>
    <td class="tg-uril">Operative Procedures</td>
  </tr>
  <tr>
    <td class="tg-8fiv">3</td>
    <td class="tg-pjk6">Diagnostic Procedures</td>
    <td class="tg-8fiv">8</td>
    <td class="tg-pjk6">Other Therapeutic Procedures</td>
  </tr>
  <tr>
    <td class="tg-8fiv">4</td>
    <td class="tg-pjk6">Laboratory Procedures</td>
    <td class="tg-8fiv">9</td>
    <td class="tg-pjk6">Administration</td>
  </tr>
</table>



#### 2.Read Code - Diagnoses
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-uril{color:#000000;border-color:#000000;text-align:left}
.tg .tg-h8n2{font-weight:bold;color:#000000;border-color:#000000;text-align:left}
.tg .tg-4yk5{font-weight:bold;background-color:#ecf4ff;color:#000000;border-color:#000000;text-align:center}
.tg .tg-q4o2{font-weight:bold;color:#333333;border-color:#000000;text-align:left}
.tg .tg-clsj{color:#333333;border-color:#000000;text-align:left}
.tg .tg-7j3r{font-weight:bold;color:#333333;border-color:#000000;text-align:left;vertical-align:top}
.tg .tg-on52{color:#333333;border-color:#000000;text-align:left;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-4yk5" colspan="4">Diagnoses</th>
  </tr>
  <tr>
    <td class="tg-q4o2">A</td>
    <td class="tg-uril">Infectious and,Parasitic Diseases</td>
    <td class="tg-h8n2">L</td>
    <td class="tg-uril">Pregnancy, Childbirth etc</td>
  </tr>
  <tr>
    <td class="tg-q4o2">B</td>
    <td class="tg-clsj">Neoplasms</td>
    <td class="tg-q4o2">M</td>
    <td class="tg-clsj">Skin &amp; Subcutaneous Tissue Diseases</td>
  </tr>
  <tr>
    <td class="tg-q4o2">C</td>
    <td class="tg-clsj">Endocrine,,Nutrition and Metabolic Disorders</td>
    <td class="tg-q4o2">N</td>
    <td class="tg-clsj">Musculoskeletal &amp; Connective Tissue Diseases</td>
  </tr>
  <tr>
    <td class="tg-7j3r">D</td>
    <td class="tg-on52">Blood and,Blood-forming Organs</td>
    <td class="tg-7j3r">P</td>
    <td class="tg-on52">Congenital Anomalies</td>
  </tr>
  <tr>
    <td class="tg-7j3r">E</td>
    <td class="tg-on52">Mental Disorders</td>
    <td class="tg-7j3r">Q</td>
    <td class="tg-on52">Perinatal Conditions</td>
  </tr>
  <tr>
    <td class="tg-7j3r">F</td>
    <td class="tg-on52">Nervous System,&amp; Sense Organs Diseases</td>
    <td class="tg-7j3r">R</td>
    <td class="tg-on52">Symptoms, Signs and Ill-defined conditions</td>
  </tr>
  <tr>
    <td class="tg-7j3r">G</td>
    <td class="tg-on52">Circulatory System,Disorders</td>
    <td class="tg-7j3r">S</td>
    <td class="tg-on52">Injury and Poisoning</td>
  </tr>
  <tr>
    <td class="tg-7j3r">H</td>
    <td class="tg-on52">Respiratory System,Diseases<br></td>
    <td class="tg-7j3r">T</td>
    <td class="tg-on52">Cause of Injury and Poisoning</td>
  </tr>
  <tr>
    <td class="tg-7j3r">J</td>
    <td class="tg-on52">Digestive System,Diseases</td>
    <td class="tg-7j3r">U</td>
    <td class="tg-on52">[X] External Causes of Morbidity and Mortality</td>
  </tr>
  <tr>
    <td class="tg-7j3r">K</td>
    <td class="tg-on52">Genitourinary,System Diseases</td>
    <td class="tg-7j3r">Z</td>
    <td class="tg-on52">[V] Supplementary factors influencing health status or contact with the Health services other than for illness</td>
  </tr>
</table>


#### 3.Read Code - How they are orgnasied
Within the chapters, terms are organised hierarchically, the higher up the hierarchy the less specific the codes. Full stops are used as ‘padding’ characters to ensure that all codes contain 5 characters. For example:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-qtf5{border-color:#000000;text-align:left}
</style>
<table class="tg">
  <tr>
    <th class="tg-qtf5">1…..</th>
    <th class="tg-qtf5">History / symptoms</th>
  </tr>
  <tr>
    <td class="tg-qtf5">17…</td>
    <td class="tg-qtf5">Respiratory symptoms</td>
  </tr>
  <tr>
    <td class="tg-qtf5">171..</td>
    <td class="tg-qtf5">Cough</td>
  </tr>
  <tr>
    <td class="tg-qtf5">1714</td>
    <td class="tg-qtf5">Productive cough -green sputum</td>
  </tr>
</table>


<figure class="center"> <img src="{{ site.url }}{{ site.baseurl }}/images/background/read_hier.png" style="width: 450px" align="middle">


#### 4.Issues
1. 'On browsing it was noted that depression was entered under different code stems. For example, Read codes for mental disorders began with the stem ‘E’; however, relevant codes were also found under ‘signs and symptoms’ with the stem ‘R’ or under examination with the stem ‘2’. The most common code stems were noted' - Creating medical and drug code lists to identify cases in primary care databases.




### Glossary
**CCGs** - <a href='https://www.nhscc.org/ccgs/'>Clinical Commission Groups</a> commission most of the hospital and community NHS services in the local areas for which they are responsible. Commissioning involves deciding what services are needed for diverse local populations, and ensuring that they are provided.

**CRS** - Clinical Record System or Care Records Service?

**CSUs** - Commissioning Support Units provide CCGs with external support, specialist skills and knowledge to support them in their role as commissioners, including business intelligence services, clinical procurement services, business support services such as human resources, payroll, procurement of goods and services and some aspects of informatics.

**ELFT** - <a href='https://www.elft.nhs.uk/'>East London NHS Foundation Trust</a> (formerly known as East London and The City University Mental Health NHS Trust) was formed in April 2000. It provides mental health and community health services in East London and specialist services to a wider region.


**EMIS** - EMIS Health, formerly known as <a href='https://www.emishealth.com/'>Egton Medical Information Systems</a>, supplies electronic patient record systems and software used in primary care in England. It claims that more than half of GP practices across the UK use EMIS software.


**GP** - General practitioner, a family doctor who works from a local surgery to provide medical advice and treatment to patients registered on their list .

**HLP** - <a href='https://www.healthylondon.org/'>Healthy London Partnership</a> works with its partners to transform, connect and improve health and care so everyone in the capital can live healthier lives.

**RiO** - The electronic patient record system which holds information about referrals, appointments and clinical information.
