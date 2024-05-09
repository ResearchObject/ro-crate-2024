---
page_id: datalake
title: KEOD Data Lake
description: Knowledge Enhanced Digital Objects (KEOD) is an experimental approach of building a data lake using a combination of knowledge graphs, RO-Crate and PID records.
url: https://github.com/luoyu357/KEDODataLake
---

# KEOD Data Lake


Knowledge Enhanced Digital Objects ([KEOD](https://github.com/luoyu357/KEDODataLake)) is an experimental approach of building a data lake using a combination of knowledge graphs, RO-Crate and PID records. 

A KEDO PID is a Handle that identifies a KEDO Object, described using a KEDO RO-Crate. This crate again has _internal RO-Crate_s as parts, which records a combination of _Features_ and _Insights_. The distinction is that features are mainly fixed at digital object creation and considered directly describing the object's nature, while insights can be discovered later from further processing and linkage.

Files in a KEDO RO-Crate are stored locally, and each recorded with a Handle PID within the crate. In this KEOD setup of multiple graphs then form a single knowledge unit.

## Resources

* Yu Luo (2022): [Knowledge enhanced digital objects](https://www.proquest.com/docview/2763290077) (Doctoral dissertation, Indiana University)
* Conference paper: <https://doi.org/10.1109/CCGridW59191.2023.00064>
* Source: <https://github.com/luoyu357/KEDODataLake>

<!--
[![datalake logo](../assets/img/datalake.svg)](https://datalake.org/)

[datalake](https://reliance.rohub.org/) (EXAMPLE-ACRONYM), is a...

datalake uses RO-Crate for ... as ....

datalake works with Project X, .....

![datalake screenshot with RO-Crate(../assets/img/datalake-screenshot.png)


## RO-Crate in datalake

(Show practically how RO-Crate is used, link to profile of RO-Crate, etc.)

The datalake API supports [RO-Crate export](http://datalake.org/docs/ro-crate) as...

datalake also plans to do...

datalake:
```
curl -H "Accept: application/ld+json" https://datalake.com/ro-crate/a72f314d

{
  "@context": { … },
  "@graph": [
   …
    {
      "@id": "./",
      "hasPart": […],
      "@type": "Dataset",
    }
   …
}
```


## Resources

* [datalake Homepage](https://datalake.org/)
* [datalake documentation](https://datalake.org/docs/)
* [RO-Crate profile for datalake](https://datalake.org/crate-profile)
* [datalake Tutorials](https://datalake.org/docs/tutorial)
* [datalake presentation](http://datalake.org/)

## Publications

Alice Land, Bob Bunny (2020):  
**datalake and RO-Crate**.  
_datalake Journal_ **0**(1)
<https://doi.org/10.1234/datalake>  
[[preprint](http://datalake.com/preprint.pdf)]

-->
