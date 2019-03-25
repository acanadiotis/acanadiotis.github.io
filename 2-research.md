---
layout: default
title: Research
permalink: /research/
---
# Research

Today, we have in our hands massive amounts of data, but we are not able to process them efficiently and extract useful insights out of them.
In the meanwhile, the sources of data grow both in size, variety, and heterogeneity.
The Internet of Things, genomics and bio-medical applications, high-energy physics, astronomy, and many more fields generate an unprecedented amount of data that often need to be combined in order to construct meaningful information.
On top of that, data analysts require support for different types of queries, even if they are performed on top of the same data.

My research focuses on bridging the heterogeneity across different data sources and on adapting the system configuration to the requirements of each end-user application.
Throughout my career so far, I have worked on standardising middleware frameworks in order to enable interoperability across applications, on bridging the network heterogeneity in order to enable device-to-device communication at extreme scale for the Internet of Things, and on elastic infrastructures to adapt resource scheduling to the application requirements at runtime.
My vision is to jointly optimise data analysis with resource scheduling in order to provide adaptive systems to the users.
In the following, I give a short overview of some projects that I have worked on in this course.

## Unified network control in the Internet of Things
The Internet of Things consists of billion of devices connected over different types of networks.
Due to this network heterogeneity, many times it is not possible for end-to-end devices to open a direct communication channel.
My research in software-defined wireless sensor networks aims in bridging the gap across IoT devices.
For this reason, I have designed and developed a network operating system for the IoT which enables communication of IoT devices over software-defined wireless and wired networks.
On top of this infrastructure, I have studied the optimal allocation of wireless sensor nodes to perform in-network Map/Reduce in order to offload the network from sending all data to the cloud. Details on this project can be found [here.](https://github.com/sdnwiselab)

## Elastic scale-up data management systems
Data management systems are continuously migrated to the cloud in order to exploit the elasticity provided by it and adjust their resource allocation to the requirements of their workload.
Current solutions typically treat elasticity in a scale-out fashion by adding or removing resources at the level of a server instance.
However, this approach can incur significant overheads for stateful applications, like transactional database engines.
My research provides a different angle by proposing scale-up elasticity for short-lived workload changes.
I have designed and implemented a system that enables applications running inside virtual machines to perform fine-grained resource allocation in big multi-socket, multi-core servers.
This project has been built considering a transactional engine, which can be found [here.](https://github.com/epfl-dias/trireme)

## Standardised middleware technologies
Interoperability is a critical dimension of content distribution systems, especially to the ones in the multimedia industry.
In this case, several stakeholders with different levels of ownership and intellectual property need to access and benefit from multimedia content.
MPEG-M is a standard middleware technology that provides specification for APIs, engines and protocols that enable the creation of added value multimedia services through a set of distributed, elementary services.
I have contributed to the design, specification and implementation of such services and engines during the standardisation of the second version of MPEG-M (ISO/IEC 23006).
Details about this project and its current status can be found [here.](https://mpeg.chiariglione.org/standards/mpeg-m)
