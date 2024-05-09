---
page_id: dataplant
title: Data Plant
description: DataPLANT`s mission is to provide a sustainable and well annotated data management platform for plant sciences.
url: https://nfdi4plants.org/content/learn-more/annotated-research-context.html
---

# DataPlant

[DataPlant](https://nfdi4plants.org/) is implementing [Annotated Research Context (ARC)](https://nfdi4plants.org/content/learn-more/annotated-research-context.html), an RO-Crate profile that combines the Investigation Study Assay model ([ISA](https://isa-specs.readthedocs.io/en/latest/isamodel.html)) and the Common Workflow Language ([CWL](https://www.commonwl.org/)) to capture a range from single experimental setups to complex experimental designs. 

In ARC, files are managed in a git repository with a fixed structure following the ISA model, in addition to metadata in an Excel spreadsheet. The [arcCommander](https://github.com/nfdi4plants/arcCommander) tool can help with managing this structure, while the tool [arc--to-roc](https://github.com/nfdi4plants/arc-to-roc) can inspect the structure to generate an RO-Crate metadata file.
The [ARC specification](https://github.com/nfdi4plants/ARC-specification/blob/main/ARC%20specification.md#appendix-conversion-of-arcs-to-ro-crates) allows augmentation by adding an explicit `ro-crate-metadata.json` to the ARC.

<!--
[![dataplant logo](../assets/img/dataplant.svg)](https://dataplant.org/)

[dataplant](https://reliance.rohub.org/) (EXAMPLE-ACRONYM), is a...

dataplant uses RO-Crate for ... as ....

dataplant works with Project X, .....

![dataplant screenshot with RO-Crate(../assets/img/dataplant-screenshot.png)


## RO-Crate in dataplant

(Show practically how RO-Crate is used, link to profile of RO-Crate, etc.)

The dataplant API supports [RO-Crate export](http://dataplant.org/docs/ro-crate) as...

dataplant also plans to do...

dataplant:
```
curl -H "Accept: application/ld+json" https://dataplant.com/ro-crate/a72f314d

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

* [dataplant Homepage](https://dataplant.org/)
* [dataplant documentation](https://dataplant.org/docs/)
* [RO-Crate profile for dataplant](https://dataplant.org/crate-profile)
* [dataplant Tutorials](https://dataplant.org/docs/tutorial)
* [dataplant presentation](http://dataplant.org/)

## Publications

Alice Land, Bob Bunny (2020):  
**dataplant and RO-Crate**.  
_dataplant Journal_ **0**(1)
<https://doi.org/10.1234/dataplant>  
[[preprint](http://dataplant.com/preprint.pdf)]

-->
