---
title: "KNIFE - Code"
layout: textlay
excerpt: "KNIFE - Code"
sitemap: false
permalink: /code/
---

## Code

### 1. Diabetes-PracticeFusion: 
- Source: https://www.kaggle.com/c/pf2012-diabetes
- Dataset: see [here]({{ site.baseurl }}/downloads/Diabetes-PracticeFusion/)
- Solution:
-- mapped complicating conditions with their ICD9, together with other features to do feature selection;
-- grouped by features; 
-- built model for each group (some are boosted regression trees, some are random foresets), and validated each group's model as a --classfication problem (whether the patient has diabetes).
