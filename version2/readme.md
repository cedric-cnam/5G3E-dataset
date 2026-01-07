## 5G3E Dataset

**Version:** 2  
**Release Date:** Dec 8, 2025

The first edition of the dataset contains time-series system metrics related to the observation of multiple resources involved in 5G network operation: radio, computing, and network resources. The variety of collected features ranges from radio front-end metrics to physical server, from operating system to network function metrics. A few thousand such features are collected, grouped by resource type and/or node type. For more details, check the version-1 [readme.md](../version1/README.md) file.

The second edition of the 5G3E dataset is assembled thanks to an updated testbed, which introduces a fully cloud-native, containerized deployment of the complete 5G stack. While the first version of the testbed containerized only the core network on Kubernetes, V2 extends this approach to include both the Core Network (CN) and the Radio Access Network (RAN). This full-stack containerization provides access to a far richer and more granular set of end-to-end performance and operational metrics. The current iteration of the dataset contains time-series system metrics similar to those in Version 1 but features expanded metric coverage, the time interval for the collection is 300ms.

**Key Improvements in V2**

- V2 utilizes the cloud-native 5G Standalone (SA) Core Network architecture by containerizing all the network functions with the integration of Kubernetes orchestrator, a critical shift from the 4G-anchored Non-Standalone (NSA) implementation used in V1.

- Updated Software Stack ⚙️: All major open-source components—Open5GS (Core), srsUE, and srsGNB (RAN)—have been upgraded to their latest stable versions, ensuring modern protocol compliance and features. We can on-demand, provide datasets using different open-source stacks such as OpenAirInterface, free5gc, etc.

- End-to-End Containerization 🐳: Every network function, from the Core Network (CN) components to the gNodeB (gNB) and User Equipment (UE) emulation, now runs as an independent container. This critical change enables the collection of per-container metrics and simplifies deployment/reproducibility across the entire system.

- Expanded Metrics Coverage 📊: The latest Open5GS release significantly enhances operational visibility by exposing dedicated, standardized metrics endpoints across key Core Network Functions (AMF, PCF, SMF, and UPF). This capability, compliant with the 3GPP performance measurement standard (TS 28.552), is crucial for defining and assuring the 5G Key Performance Indicators (KPIs) specified in TS 28.554, allowing for proactive performance monitoring and service assurance.

## **Availability**

A sample of the dataset corresponding to Day 10 of the collected training metrics is available for download.

**Sample Dataset**:

    Files: 96
    Format: csv,json
    Duration: 10 mins
[Click here for more information](./SampleData/readme.md)


| Metric Level | CPU | Memory | Network | Disk | Function level | Timeseries/ node (upto) | Nb. targets |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | 
| Physical | 300 – 1100 | 37 – 60 | 170 – 920 | 42 – 296 | - | 1211-2826 | 7 |
| Container | 2 – 5 | 10 – 15 | 8 – 15 | 5 – 7 | - | 695-1010 | 88 |
| NFV* | - | - | - | - | 20 – 25 | 13-28 | 4 |



**Full Dataset Download Links**
> [!NOTE] 
> The links are password protected, please [contact](#contact) us to gain access.
> The size of each day is approximately 4 GiB.

[Day1](https://box.roc.cnam.fr/index.php/s/EarkQpZbxR9ke7G)

[Day2](https://box.roc.cnam.fr/index.php/s/YzwWayWsJaPMByB)

[Day3](https://box.roc.cnam.fr/index.php/s/638YgYPQZKdtRBN)

[Day4](https://box.roc.cnam.fr/index.php/s/EjnRgTjJ9bzBBgD)

[Day5](https://box.roc.cnam.fr/index.php/s/6KebiieXCdKqM9Z)

[Day6](https://box.roc.cnam.fr/index.php/s/Zr8i7D5cEnXw9yW)

[Day7](https://box.roc.cnam.fr/index.php/s/o7EqTFbpKjj9yg4)

[Day8](https://box.roc.cnam.fr/index.php/s/oaBt2oAafTnLk3C)

[Day9](https://box.roc.cnam.fr/index.php/s/LKEmJ2KPKMzj3c7)

[Day10](https://box.roc.cnam.fr/index.php/s/JMoyneT4FeL3N7q)

[Day11](https://box.roc.cnam.fr/index.php/s/wAMFnwywNyPntSW)

[Day12](https://box.roc.cnam.fr/index.php/s/8zM5GY2wRiSJ85o)

[Day13](https://box.roc.cnam.fr/index.php/s/RwbfQy92eb2RESs)

[Day14](https://box.roc.cnam.fr/index.php/s/3BYENGRBxBqAJer)



**Custom demands**

We can support custom requirements, targeting specific scenarios such as:

- Integration of Non-Terrestrial Networks (NTN)
- Support for additional 5G functions
- Implementation of disagregated RAN settings
- Enable multiple 5G core instances
- Hybrid setup with real and emulated UEs
- Integration with closed loop automation subsystems such as: 
    - Anomaly detection algorithms
    - Data pipeline systems
    - Autonomous orchestrators

We are open to support other custom requirements.

**ACKNOWLEDGEMENT**

This dataset is created and maintained thanks to the support of the following public-funded research projects:

- ANR TREES (TowaRds Energy Efficient diStributed learning for 6G): https://trees.roc.cnam.fr. Contract nb: ANR-24-IAS1-0004.
- PIIEC ME/CT PART
- ANR COCO 5G: https://coco5g.roc.cnam.fr. Contract nb: ANR-22-CE25-0016.

## **Contact**

Write us if need any additional information. Email: masoud.baharlouei AT cnam DOT fr and naresh.modina AT cnam DOT fr