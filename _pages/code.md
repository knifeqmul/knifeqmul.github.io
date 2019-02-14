---
title: "KNIFE - Code"
layout: textlay
excerpt: "KNIFE - Code"
sitemap: false
permalink: /code/
---

## Code

### 1. Diabetes-PracticeFusion: 
<oi>
<li> Source: https://www.kaggle.com/c/pf2012-diabetes</li>
<li> Dataset: see [here]({{ site.baseurl }}/downloads/Diabetes-PracticeFusion/)</li>
<li> Solution:<ui>
<li> mapped complicating conditions with their ICD9, together with other features to do feature selection;</li>
<li> grouped by features; </li>
<li> built model for each group (some are boosted regression trees, some are random foresets), and validated each group's model as a --classfication problem (whether the patient has diabetes).</li>
  </ui></li>
</oi>
