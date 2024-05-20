---
page_id: life-monitor
redirect_from: life_monitor
title: Life Monitor
description: Life Monitor is a testing and monitoring service for computational workflows being developed as part of the EOSC-Life project. It aims to facilitate the execution, monitoring and sharing of workflow tests over time, allowing to detect deviations from expected workflow operation and provide useful feedback to the workflow authors
image: life_monitor.png
domains: [biomedical_science, medicine, omics]
tasks: [conduct_research, software_development]
roles: [researcher, software_developer]
---
## Life Monitor
[Life Monitor](https://crs4.github.io/life_monitor/) is a testing and monitoring service for computational workflows being developed as part of the [EOSC-Life](https://www.eosc-life.eu/) project. It aims to facilitate the execution, monitoring and sharing of workflow tests over time, allowing to detect deviations from expected workflow operation and provide useful feedback to the workflow authors for maintaining and improving their work.

Life Monitor uses RO-Crate as an exchange format for the description of test suites associated with workflows. To this end, the Life Monitor team is developing [an extension to the Workflow RO-Crate specification](https://github.com/crs4/life_monitor/wiki/Workflow-Testing-RO-Crate) to support the inclusion of metadata related to the testing of computational workflows stored in the crate.

![](https://www.researchobject.org/ro-crate/assets/img/ro-crate-exchange.png)

As shown in the above picture, Life Monitor gets metadata about the workflow, including test suites, from the workflow’s RO-Crate, and uses them to communicate with the relevant CI services. Test outcomes are then collected and exposed via a REST API.
