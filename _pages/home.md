---
title: "KNIFE - Home"
layout: homelay
excerpt: "Knowledge Discovery from Health Use Data"
sitemap: false
permalink: /
---


**KNIFE (Knowledge Discovery from Health Use Data)** is a Turing Institute funded project led by Dr William Marsh, with co-investigators Prof Norman Fenton, Prof Martin Neil, and Dr John Robson.

The increasing use and capability of Electronic Health Record (EHR) systems has made available large databases of patient records, linked across different health providers. These databases contain information about patients’ use of the different health services, treatments and prescriptions. The data, collected for clinical management or financial reporting, has many actual and potential uses including discovering causes, optimising health delivery, allocating resources and choosing treatment. However, there are both practical and technical challenges to overcome before these benefits can be achieved. The overall objective of the project is to lay the foundations for a transformative approach to patient-linked health data, making it accessible for both medical and data science researchers to fully exploit. We will achieve this by working with two groups who are custodians of data of this type in East London.

For full details see [here]({{ site.baseurl }}/downloads/Turing-proposal-marsh-4pages.pdf).




#### **Task 1: Data Description at Several Levels of Abstraction.**

*  Create a simplified model of the data generation process, covering the organisations involved, using a mix of text and diagrams.
*  Create a semantic schema, using web ontology techniques or related techniques. We will also investigate the use and role of the medical ontologies used to tag data (primarily SNOMED).
*  Investigate the mapping between the semantic schema and the storage schema, its use for data access and the potential for automating its construction.

This task will result in a description of the data that can be shared with potential collaborators. A complete data dictionary may not be necessary if the same concepts recur in different parts of the data.



#### **Task 2: Generative Model. Building on the work of task 1, this task will:**

*  Develop a sequence of generative models, based on the description of the data generation process, forming the most detailed ‘executable’ description of the data.
*  Use the models to generate synthetic datasets and, if possible, compare the descriptive statistics, using this to refine the generative model.

This task will result in a ‘data sandpit’ to allow other researchers to evaluate analytical and learning algorithms. The true values of many of the parameters used in the generator will be unknown, so (even if the structure is correct) the synthetic data will not fully correspond to the actual data. However, researchers will be able to modify and rerun the generator, creating a test bed for algorithms. 


