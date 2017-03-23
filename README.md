# bpmn-models
some bpmn models, home-made or taken from the literature

If you use the models, please refer to the original publication when available. The objective is only to have a place with some models for evaluation purposes, not to get credit for others' work.

This repository takes its origin as a side-effect of the [PARDI project](http://pardi.enseeiht.fr), funded by the French National Agency for Research.

![ANR logo](logo-anr-small.png)

## model 0001-v0001

**Examination management system**

[model](models/e0001v0001.bpmn) / [picture](pictures/e0001v0001.png)

Example taken and slightly modified from: 

*F. Chevrou, A. Hurault, and P. Queinnec: On the Diversity of Asynchronous Communication. FAC 28 2016*
([link](http://doi.org/10.1007/s00165-016-0379-x))
Modifications:
- add parallelism- add inobservable tasks for taking coffee (in addition to sending the corresponding invitation) and working on the exam

## model 0002-v0001

**Shift worker schedulling model**

[model](models/e0002v0001.bpmn) / [picture](pictures/e0002v0001.png)

Example taken and slightly modified from: 

*Jeremy W. Bryans, Wei Wei: Formal Analysis of BPMN Models Using Event-B. FMICS 2010*
([link](http://doi.org/10.1007/978-3-642-15898-8_3))Modifications:- add a merge gateway- modify the data flows and add data-related annotations
- remove the timer on getting the response from workers