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



<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="5000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">

        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/background/databases.png" width="60%" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/dataGeneration.jpg"  width="80%" alt="Slide 2" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/sem.png"  width="90%" alt="Slide 3" />
        </div>

    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>







#### **Task 1: Data Description at Several Levels of Abstraction.**

*  Create a simplified model of the data generation process, covering the organisations involved, using a mix of text and diagrams.
*  Create a semantic schema, using web ontology techniques or related techniques. We will also investigate the use and role of the medical ontologies used to tag data (primarily SNOMED).
*  Investigate the mapping between the semantic schema and the storage schema, its use for data access and the potential for automating its construction.

This task will result in a description of the data that can be shared with potential collaborators. A complete data dictionary may not be necessary if the same concepts recur in different parts of the data.



#### **Task 2: Generative Model. Building on the work of task 1, this task will:**

*  Develop a sequence of generative models, based on the description of the data generation process, forming the most detailed ‘executable’ description of the data.
*  Use the models to generate synthetic datasets and, if possible, compare the descriptive statistics, using this to refine the generative model.

This task will result in a ‘data sandpit’ to allow other researchers to evaluate analytical and learning algorithms. The true values of many of the parameters used in the generator will be unknown, so (even if the structure is correct) the synthetic data will not fully correspond to the actual data. However, researchers will be able to modify and rerun the generator, creating a test bed for algorithms. 



#### **Task 3: Data Use, Knowledge Elicitation and Analysis Methods.**

*  Elicit from data custodians the uses of the data and categorise the data analytic challenges. We will consider both what is currently possible and what might be achieved in future.
*  Review available statistical / ML (including SRL) techniques against the data analytic requirements.
*  Investigate how causal knowledge could be elicited and modelled for data of this complexity (with examples, if possible).
*  If possible, carry out ‘proof of concepts’ analyses, using either real or synthetic data (Task 2).

The task will result in a clearer definition in the data analysis and knowledge modelling research needs, distinguishing these from what can be achieved with current techniques. 



#### **Task 4: Practical Data Handling issues.**

*  Use the results of task 1 to investigate the data quality issues, including clarifying the concept of missing data given the clinical discretion in choosing which values to record.
*  Catalogue the range of data wrangling issues encountered in practical and determine the type of knowledge needed to provide automatic assistance.

This task will result in a clear set of challenges for improving the efficiency of data analysis, using current analysis techniques.


#### **Task 5: Outreach and consortium building.**

This task will be to build a consortium of researcher to collaborate on future work. Guided by the leadership of the Turing Health Programme, we will identify and contact potential collaborators. Workshops (or a workshop) will be run to share ideas and we expect to prepare follow-up proposals. 




