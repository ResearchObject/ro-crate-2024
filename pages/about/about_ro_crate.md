---
title: About RO-Crate
sidebar: about
---

# About RO-Crate

## What is an RO-Crate?

An RO-Crate is a [Research Object](background#research-object-background) (or _RO_) formed of a collection of data (a _crate_) and a special `ro-crate-metadata.json` file which describes the collection.

The collection may contain any kind of research data - papers, data files, software, references to other research, and so on. It may be a folder full of files, an abstract grouping of connected references, or a combination of both.

The `ro-crate-metadata.json` file (also known as the _RO-Crate Metadata Document_) is a plain text file, readable by humans and machines, that includes metadata for each item within the collection - the authors, license, identifier, and so on. Any folder can be turned into an RO-Crate by adding an `ro-crate-metadata.json` file.

Researchers can distribute their work as an RO-Crate to ensure their data travels with its metadata, so that key components are correctly tracked, archived, and attributed. [something about reproducibility]

RO-Crate uses the [JSON-LD](https://json-ld.org) format, which is based on [JSON](https://www.json.org/json-en.html). The `ro-crate-metadata.json` file can be written by hand or by using one of the existing [tools](./pages/tools). Some workflow managers (such as Galaxy) support exporting RO-Crates from their web interface.

Below is an example of an `ro-crate-metadata.json` file, which describes rainfall data published by an Australian institute under a Creative Commons license:

```
{
  "@context": "https://w3id.org/ro/crate/1.2-DRAFT/context",
  "@graph": [
    {
      "@id": "ro-crate-metadata.json",
      "@type": "CreativeWork",
      "conformsTo": {"@id": "https://w3id.org/ro/crate/1.2-DRAFT"},
      "about": {"@id": "./"}
    },
    {
      "@id": "./",
      "@type": "Dataset",
      "name": "Example dataset for RO-Crate specification",
      "description": "Official rainfall readings for Katoomba, NSW 2022, Australia",
      "datePublished": "2022-12-01",
      "publisher": {"@id": "https://ror.org/04dkp1p98"},
      "license": {"@id": "http://spdx.org/licenses/CC0-1.0"},
      "hasPart": [
        {"@id": "data.csv"}
      ]
    },
    {
      "@id": "data.csv",
      "@type": "File",
      "name": "Rainfall data for Katoomba, NSW Australia February 2022",
      "encodingFormat": "text/csv",
      "license": {"@id": "https://creativecommons.org/licenses/by-nc-sa/3.0/au/"}
    },
    {
      "@id": "https://ror.org/04dkp1p98",
      "@type": "Organization",
      "name": "Bureau of Meteorology",
      "description": "Australian Government Bureau of Meteorology",
      "url": "http://www.bom.gov.au/"
    },
    {
      "@id": "https://creativecommons.org/licenses/by-nc-sa/3.0/au/",
      "@type": "CreativeWork",
      "name": "CC BY-NC-SA 3.0 AU",
      "description": "Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Australia"
    }
  ]
}
```

See [Walkthrough of an RO-Crate](../../_specification/1.2-DRAFT/introduction#walkthrough-an-initial-ro-crate) for an explanation of each element of the file, or [Tutorials](TODO) for a hands-on introduction.

## Why should I use RO-Crate?

[this is heavily inspired by https://citation-file-format.github.io, CC-BY The Citation File Format Contributors, and could probably use some more tweaking to suit RO-Crate users]

It is very easy to correctly cite a paper: all the necessary information (metadata) can be found on the title page or the article website. Software and datasets have no title page, the relevant information is often less obvious.

People who want to cite your work may ask questions like:

* What label should I use to uniquely identify the version of the data I have used?
* What is the appropriate set of people that should be cited as authors for this dataset?

The person who wants to cite your data will probably not be able to answer these questions accurately and consistently themselves, but you can! Give them all the right information in an `ro-crate-metadata.json` file, and they can cite your software correctly.

Also, if you publish your RO-Crate in an archive or registry, they (or their systems) can re-use the citation metadata from your `ro-crate-metadata.json` file.

## Who is RO-Crate for?

RO-Crate is for everyone! The RO-Crate effort brings together practitioners from very different backgrounds, and with different motivations and use-cases. Among our core target users are:

* researchers engaged with computation and data-intensive, workflow-driven analysis
* digital repository managers and infrastructure providers
* individual researchers looking for a straight-forward tool or how-to guide to “FAIRify” their data
* data stewards supporting research projects in creating and curating datasets.

RO-Crates are suitable for any domain, as they are general-purpose and can contain arbitrary data, but they can also be specialised through the use of [RO-Crate Profiles](TODO). Profiles define additional conventions, types and properties that RO-Crates may use within a particular domain, application or framework. For example, the [Workflow RO-Crate profile]() provides guidance on constructing RO-Crates that describe executable workflows.

We continue to gather [use cases](./pages/use_cases), please help us by adding more.

## About the RO-Crate Project

[needs simplification]

RO-Crate is a community effort to establish a lightweight approach to packaging research data with their metadata. It is based on schema.org annotations in JSON-LD, and aims to make best-practice in formal metadata description accessible and practical for use in a wider variety of situations, from an individual researcher working with a folder of data, to large data-intensive computational research environments.

## More information

Check the [FAQ](./faq) for answers to common questions.

Visit the [Tutorials](TODO) page for hands-on introductions to RO-Crate and common associated tools and profiles.

Visit the [Use Cases](../use_cases) page to browse projects using RO-Crate, or find relevant information for your [domain](../domains), [project role](../roles), or [task](../tasks).

Read the [Background](./background) page to learn about the history of RO-Crate and its predecessors.
