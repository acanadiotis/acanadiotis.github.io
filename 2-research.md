---
layout: default
title: Research
permalink: /research/
---
# Research

Today, we have in our hands massive amounts of data, but we are not able to process them efficiently and extract useful insights out of them.
In the meanwhile, both the data sources and the workloads grow in size, variety, and heterogeneity.
Internet of Things, genomics and bio-medical applications, high-energy physics, astronomy, and many more fields generate an unprecedented amount of data that often need to be combined in order to construct meaningful information.
On top of that, data analysts require support for different types of queries, even if they are performed on top of the same data.

My research focuses on bridging the heterogeneity across different data sources, workloads and systems and on adapting the system resource allocation to the requirements of each application.
Throughout my career so far, I have worked on standardising middleware frameworks in order to enable interoperability across applications, on bridging the network heterogeneity in order to enable device-to-device communication at extreme scale for the Internet of Things, and on elastic infrastructures to adapt resource scheduling to the workload requirements at runtime.
My vision is to jointly optimise data processing algorithms execution with resource scheduling in order to build systems which are adaptive to underlying resource available in par with the workload requirements.
In the following, I give a short overview of some projects that I have worked on in so far with several colleagues throughout my career.

## Fresh data processing
Data freshness has become a major requirement of modern data warehousing systems, which consider data being ingested by a transactional workload and, then, analyzed shortly afterwards by analytical queries.
This area, typically referred to as Hybrid Transactional Analytical Processing (HTAP), focuses on the data freshness guarantees provided by the related systems and challenges the way transactional and analytical queries are executed over the same database.
In this line of work, we have modeled HTAP as a resource management problem, where a transactional and an analytical engine are competing for resources.
By elastically trading resources between the engines, this work shows that there exists an adaptive system design, which can be elastically constructed at runtime based on the workload and the resource availability.
This approach has been applied in both CPU and GPU-based engines. 

## Scale-up elasticity for stateful systems
A transactional database engine has to maintain a consistent state throughout the workload execution.
This becomes particularly challenging in the face of variations in the workload, where the engine has to elastically adapt its resource allocation to meet its performance SLAs.
Scale-out elasticity, which is typically used in this case, has overheads in maintaining the state as partitions change due to extensive state migration and distributed transaction coordination.
These overheads are only ammortized when the variation lasts long enough to compensate for the overheads.
Instead, this approach proposes an elastic scale-up system design and shows that it is beneficial for short-lived workload variations.
Moreover, this approach introduces a new spot instance model for the cloud, where stateful engines are deployed within virtual machines which have minimum and maximum resource guarantees and resources are traded across VMs with minimal overheads.   
This project has been built considering a transactional engine, which can be found [here](https://github.com/epfl-dias/trireme), whereas the work has been funded by Huawei. 

## Unified network control in the Internet of Things
The Internet of Things consists of billion of devices connected over different types of networks.
Due to this network heterogeneity, many times it is not possible for end-to-end devices to open a direct communication channel.
My research in software-defined wireless sensor networks aims in bridging the gap across IoT devices.
For this reason, I have designed and developed a network operating system for the IoT which enables communication of IoT devices over software-defined wireless and wired networks.
On top of this infrastructure, I have studied the optimal allocation of wireless sensor nodes to perform in-network Map/Reduce in order to offload the network from sending all data to the cloud. Details on this project can be found [here.](https://github.com/sdnwiselab)

## Standardised middleware technologies
Interoperability is a critical dimension of content distribution systems, especially to the ones in the multimedia industry.
In this case, several stakeholders with different levels of ownership and intellectual property need to access and benefit from multimedia content.
MPEG-M is a standard middleware technology that provides specification for APIs, engines and protocols that enable the creation of added value multimedia services through a set of distributed, elementary services.
I have contributed to the design, specification and implementation of such services and engines during the standardisation of the second version of MPEG-M (ISO/IEC 23006).
Details about this project and its current status can be found [here.](https://mpeg.chiariglione.org/standards/mpeg-m)
