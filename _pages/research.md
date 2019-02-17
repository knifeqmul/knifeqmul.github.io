---
title: "KNIFE - Research"
layout: gridlay
excerpt: "KNIFE -- Research."
sitemap: false
permalink: /research/
---

### Review

#### 1. Problems with Data

##### 1.1 Data with censorship: 
A situation where a patient’s state is only observable during a certain period of time, or conversely, when potentially interesting events fall outside the observation period and are hence unobservable. 

##### 1.2 Irregular time-series data
Irregularity of the patient visits, certain laboratory tests are ordered annually, and other tests are performed only as
needed.

##### 1.3 Integration between different data orgins
Communication between different databases and terminology.

##### 1.4 Missing data
* The mapping between differernt changes in disease definitions and updates in the coding scheme, such as the change from ICD-9 to ICD-10 codes. For example, prediabetes did not have a corresponding ICD code until 2000
* Unobservable information: the lifestyle changes of patient, and whether the patient has taken the medicine.
* Some tests are performed only as needed, so this information is only collected when available. 


#### 2. Current applications

##### 2.1 Disease/Risk Prediction
* **Medical/disease Trajectory**: heart rate deterioration[1], Type 2 diabetes progression paths[2].
* **Multimorbidity**: e.g. the coexistence of multiple chronic diseases increases the risk of mortality[3].
* **Biomarker Discovery**: identify indicators/risk factors of a biological condition, e.g. find blood-borne biomarkers for early diagnosis of cancer[4].
  
##### 2.2 Cohort Identification
  * **Phenotype**:  a cohort (group) of patients, some of whom are more likely to have the disease. Phenotyping techniques are useful for identifying patients or populations with a given clinical characteristic from the EHRs, see review[5]. 

##### 2.3 Quantification of Intervention Effect
  * **Quantify Effects**: e.g. evaluate the effect of different treatment regimes, assessing the effectiveness of treating to four different blood pressure targets[6].
  * **Adverse Event Detection**: this term describes the detrimental effect of medical care on patient medical state. Examples include infection acquired during the treatment of a different condition, such as surgical site infection. For example, [7] identify medications caused adverse drug reactions.
  
##### 2.4 Building Evidence-Based Guideline
  * **Guideline**: Provide guidance on the optimal treatment under a particular set of conditions based on epidemiological evidence. For example, American Diabetes Association (ADA) guidelines for diabetes consist of recommendations for diagnosing the condition (e.g., a patient is considered diabetic if his or her hemoglobin A1c is >6.5), controlling the disease (patient is under control if his or her A1c is <6.5 and systolic blood pressure is <140mmHg), and prescribing interventions (lifestyle modification and therapeutic interventions).
  

---

### Temporal plans

CCG holds a data repository that links pseudonymised patient level records across health and care settings. The records replaced NHS number with pseudo ID, date of birth with age etc. It is not considered as personal data by law if this is handled in a secure enviroment. 

<img src="{{ site.url }}{{ site.baseurl }}/images/background/todo.png" style="width: 900px">



#### 1.Issues
1. Data is in CCG, while GPs are located in clinics.
2. Data is semi-structured without clear description.



#### 2.To do
1. Ontology.
2. EHR applications.
3. Causal hypothesis testing.




---
### Reference
[1] Colopy, Glen Wright, et al. 2016. Bayesian Gaussian processes for identifying the deteriorating patient. 2016 38th Annual International Conference of the IEEE Engineering in Medicine and Biology Society (EMBC).

[2] W. Oh et al. 2016. Type 2 diabetes mellitus trajectories and associated risk factors. Big Data 4, 1 (2016), 25–30.

[3] M. Mercer et al. 2009. Multimorbidity in primary care: Developing the research agenda. Family Practice 26, 2 (2009), 79–80.

[4] Yang, Yongliang, et al. 2008. Integrative genomic data mining for discovery of potential blood-borne biomarkers for early diagnosis of cancer. PloS one 3.11 (2008): e3661.

[5] C. Shivade et al. 2014. A review of approaches to identifying patient phenotype cohorts using electronic health records.
    JAMIA 21, 2 (2014), 221–230.

[6] Johnson, Kipp W., et al. 2018. Causal inference on electronic health records to assess blood pressure treatment targets: an application of the parametric g formula. Pac Symp Biocomput. Vol. 23. 2018.

[7] Haerian, K., et al. 2012. Detection of pharmacovigilance‐related adverse events using electronic health records and automated methods. Clinical Pharmacology & Therapeutics 92.2 (2012): 228-234.
