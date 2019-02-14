---
title: "KNIFE - Code"
layout: textlay
excerpt: "KNIFE - Code"
sitemap: false
permalink: /code/
---

## Code

### 1. Diabetes-PracticeFusion: 


<ol>
<li>Source: https://www.kaggle.com/c/pf2012-diabetes</li>
<li>Dataset: see <a href='https://github.com/knifeqmul/knifeqmul.github.io/tree/master/downloads/Diabetes-PracticeFusion'>[here]</a></li>
<li>Solution:
<ol style="list-style-type: lower-alpha; padding-bottom: 0;">
<li style="margin-left:2em">mapped complicating conditions with their ICD9, together with other features to do feature selection;</li>
<li style="margin-left:2em">grouped by features;</li>
<li style="margin-left:2em; padding-bottom: 0;">built model for each group (some are boosted regression trees, some are random foresets), and validated each group's model as a classfication problem (whether the patient has diabetes).</li>
</ol>
</li>
</ol>
