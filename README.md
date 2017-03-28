# bpmn-models
some bpmn models, home-made or taken from the literature

This repository takes its origin as a side-effect of the [PARDI project](http://pardi.enseeiht.fr), funded by the French National Agency for Research.

![ANR logo](logo-anr-small.png)

## files

The models are available in directory [models](models), and
graphical representation of them are in directory [pictures](pictures).

## description of the models

The set of models is described
in file [models.yaml](models.yaml)
using the [YAML format](http://yaml.org).

The (**unstable**) format of the file is:

```yaml
- id: &e0001
  name: The Name of the Example
  reference: >
    A. Alice, B. Bob, and C. Charles.
    An Example in BPMN.
    Conference/Journal, Year.
  doi: http://doi.org/xxx
  variants: [
    - id: &e0001v0001
      references: []
      doc: >
        The description of variant 0001 of example 0001 (*e0001v0001).
        This may use several lines.
      changes: [
        One line change number 1 wrt original version,
        One line change number 2 wrt original version,
        One line change number 3 wrt original version,
        etc.
      ]
    - id: &e0001v0002
      references: [*e0001v0001]
      doc: >
        The description of variant 0002 of example 0001 (*e0001v0002).
        This may use several lines.
      changes: [
        One line change number 1 wrt *e0001v0001,
        One line change number 2 wrt *e0001v0001,
        One line change number 3 wrt *e0001v0001,
        etc.
      ]
    - id: &e0001v0003
      references: [*e0001v0001,*e0001v0002]
      doc: >
        The description of variant 0003 of example 0001 (*e0001v0003).
        This may use several lines.
      changes: [
        One line change number 1 wrt *e0001v0001,
        One line change number 1 wrt *e0001v0002,
        One line change number 2 wrt *e0001v0002,
        etc.
      ]
  ]
```
