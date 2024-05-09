---
page_id: appdb
title: EGI AppDB
description: EGI’s Application Database (AppDB) has support for RO-Crate download, either as a JSON-LD metadata file or a ZIP archive.
url: https://appdb.egi.eu/
---

# EGI's Application Database

EGI's Application Database ([AppDB](https://appdb.egi.eu/)) has [support for RO-Crate](https://wiki.appdb.egi.eu/docs/integration/ro-crate/) download, either as a JSON-LD metadata file or a ZIP archive.

The AppDB RO-Crates describe the software as `SoftwareApplication` entities, similar to [CodeMeta](https://codemeta.github.io/), including link to virtual machine iamges etc. 

* [RO-Crate integration in AppDB](https://wiki.appdb.egi.eu/docs/integration/ro-crate/)
* [Example RO-Crate](https://appdb.egi.eu/store/vappliance/egi.ubuntu.20.04#) for appliance [EGI Ubuntu 20.04](https://appdb.egi.eu/store/vappliance/egi.ubuntu.20.04)


<!--
[![appdb logo](../assets/img/appdb.svg)](https://appdb.org/)

[appdb](https://reliance.rohub.org/) (EXAMPLE-ACRONYM), is a...

appdb uses RO-Crate for ... as ....

appdb works with Project X, .....

![appdb screenshot with RO-Crate(../assets/img/appdb-screenshot.png)


## RO-Crate in appdb

(Show practically how RO-Crate is used, link to profile of RO-Crate, etc.)

The appdb API supports [RO-Crate export](http://appdb.org/docs/ro-crate) as...

appdb also plans to do...

appdb:
```
curl -H "Accept: application/ld+json" https://appdb.com/ro-crate/a72f314d

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

* [appdb Homepage](https://appdb.org/)
* [appdb documentation](https://appdb.org/docs/)
* [RO-Crate profile for appdb](https://appdb.org/crate-profile)
* [appdb Tutorials](https://appdb.org/docs/tutorial)
* [appdb presentation](http://appdb.org/)

## Publications

Alice Land, Bob Bunny (2020):  
**appdb and RO-Crate**.  
_appdb Journal_ **0**(1)
<https://doi.org/10.1234/appdb>  
[[preprint](http://appdb.com/preprint.pdf)]

-->
