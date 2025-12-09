## 5G3E Dataset

**Version:** 2  
**Release Date:** Dec 8, 2025

The first edition of the dataset contains time-series system metrics related to the observation of multiple resources involved in 5G network operation: radio, computing, and network resources. The variety of collected features ranges from radio front-end metrics to physical server, from operating system to network function metrics. A few thousand such features are collected, grouped by resource type and/or node type. For more details, check the version-1 readme.md file.

The second edition of the 5G3E dataset is assembled thanks to an updated testbed, which introduces a fully cloud-native, containerized deployment of the complete 5G stack. While the first version of the testbed containerized only the core network on Kubernetes, V2 extends this approach to include both the Core Network (CN) and the Radio Access Network (RAN). This full-stack containerization provides access to a far richer and more granular set of end-to-end performance and operational metrics. The current iteration of the dataset contains time-series system metrics similar to those in Version 1 but features expanded metric coverage, the time interval for the collection is 300ms.

**Key Improvements in V2**

- V2 utilizes the cloud-native 5G Standalone (SA) Core Network architecture, a critical shift from the 4G-anchored Non-Standalone (NSA) implementation used in V1.

- Updated Software Stack ⚙️: All major open-source components—Open5GS (Core), srsUE, and srsGNB (RAN)—have been upgraded to their latest stable versions, ensuring modern protocol compliance and features.

- End-to-End Containerization 🐳: Every network function, from the Core Network (CN) components to the gNodeB (gNB) and User Equipment (UE) emulation, now runs as an independent container. This critical change enables the collection of per-container metrics and simplifies deployment/reproducibility across the entire system.

- Expanded Metrics Coverage 📊: The latest Open5GS release significantly enhances operational visibility by exposing dedicated, standardized metrics endpoints across key Core Network Functions (AMF, PCF, SMF, and UPF). This capability, compliant with the 3GPP performance measurement standard (TS 28.552), is crucial for defining and assuring the 5G Key Performance Indicators (KPIs) specified in TS 28.554, allowing for proactive performance monitoring and service assurance.

**Availability**

A sample of the dataset corresponding to Day 1 of the collected training metrics is available for download.

**Sample Dataset**:

    Files: 2
    Format: csv
    Duration: 10 mins

> [!NOTE] 
> The complete 5G3E V2 dataset will be released soon.

Write us if need any additional information. Email: masoud.baharlouei AT cnam DOT fr and naresh.modina AT cnam DOT fr

**ACKNOWLEDGEMENT**

This dataset is created and maintained thanks to the support of the following public-funded research projects:

- ANR TREES (TowaRds Energy Efficient diStributed learning for 6G): http://cancan.roc.cnam.fr. Contract nb: ANR-24-IAS1-0004.
- PIIEC ME/CT PART