---
title: "KNIFE - Task5"
layout: textlay
excerpt: "KNIFE - Task5"
sitemap: false
permalink: /task5/
---

## Task5

### Data Warehouse
#### 1. i2b2
Features: 'such as patient de-identification, natural language processing extensions, navigation using terminologies (e.g. ICD-10), combination of EHR data with genomics and a user friendly ‘drag and drop’ interface'





### Classfication
#### 1. has diabetes
<ol>
<li>Diabetes-PracticeFusion: https://www.kaggle.com/c/pf2012-diabetes</li>
<li>Dataset: see <a href='https://github.com/knifeqmul/knifeqmul.github.io/tree/master/downloads/Diabetes-PracticeFusion'>[here]</a></li>
<li>Solution:
<ol style="list-style-type: lower-alpha; padding-bottom: 0;">
<li style="margin-left:2em">mapped complicating conditions with their ICD9, together with other features to do feature selection;</li>
<li style="margin-left:2em">grouped by features;</li>
<li style="margin-left:2em; padding-bottom: 0;">built model for each group (some are boosted regression trees, some are random foresets), and validated each group's model as a classfication problem.</li>
</ol>
</li>
</ol>

#### 2. has heart disease
<ol>
<li>Heart Disease UCI: https://www.kaggle.com/ronitf/heart-disease-uci</li>
</ol>

#### 3. medical appointment no shows
<ol>
<li>Medical Appointment No Shows: https://www.kaggle.com/joniarroba/noshowappointments</li>
</ol>

