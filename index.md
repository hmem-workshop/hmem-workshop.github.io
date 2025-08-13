# Sixth Workshop on Heterogeneity and Memory Systems (HMEM 2025)

### In conjunction with [SC'25](https://sc25.supercomputing.org/), St. Louis, MO, November 17th, 2025


## Overview and scope

Heterogeneity is ubiquitous, not only in terms of processing units but also memories and networks. As heterogeneity increases, memory subsystems play an even more important role to attain performance, from their technology to the system architecture to the software management and programming model. While CPU-only compute nodes are becoming rare instances, heterogeneous memory architectures have recently emerged and revolutionized the traditional memory hierarchy. Today’s and upcoming architectures may well comprise multiple memory technologies next to DRAM, accelerators with dedicated memories, or even specific expansion cards hosting memory alone, such as: 3D-stacked memory, high-bandwidth multi-channel RAM, unified/shared memory on accelerators, Compute Express Link (CXL)-based architectures, persistent memory, or MRDIMMs.

As in previous years, the Workshop on Heterogeneous Memory Systems, now rebranded as Heterogeneity and Memory Systems (HMEM), will bring together different research efforts and expertise to the end of integrating different approaches and democratizing the use of resource heterogeneity from a memory perspective, to benefit applications not only in terms of performance, but also energy efficiency and cost trade-offs. The main goal of the workshop is to push the research frontiers forward by exchanging knowledge and debating ideas through featured talks, technical paper presentations, and interactive discussions. Overall, topics of interest include, but are not limited to:

- Resource heterogeneity (e.g., accelerators) and memory implications, including memory designs, data layouts, etc. 
- Data allocation and placement techniques in heterogeneous memory systems 
- Caching for heterogeneous memory systems 
- Programming models and tools for complex/heterogeneous memory hierarchies 
- Software-defined far memories
- Disaggregated memory and in-memory computing 
- Data movement in heterogeneous memory systems 
- Memory consistency and persistency models 
- Data structures for heterogeneous memory infrastructures 
- Abstractions and support for failure-atomicity in persistent memory 
- Emerging memory architectures and system configurations 
-	AI on heterogeneous memory systems and use of AI for heterogeneous memory systems
- Use cases, early experiences and performance evaluations


## Program 

### Featured Speaker: Torsten Hoefler (ETH Zurich). 
### ARMing GPUs: On the Memory Subsystem of Grace Hopper GH200

Abstract: Heterogeneous supercomputers have become the standard in HPC. GPUs in particular have dominated the accelerator landscape, offering unprecedented performance in parallel workloads and unlocking new possibilities in fields like AI and climate modeling. With many workloads becoming memory-bound, improving the communication latency and bandwidth within the system has become a main driver in the development of new architectures. The Grace Hopper Superchip (GH200) is a significant step in the direction of tightly coupled heterogeneous systems, in which all CPUs and GPUs share a unified address space and support transparent fine grained access to all main memory on the system. We characterize both intra- and inter-node memory operations on the Quad GH200 nodes of the new Swiss National Supercomputing Centre Alps supercomputer, and show the importance of careful memory placement on example workloads, highlighting tradeoffs and opportunities. 

Bio: Torsten Hoefler is a Professor of Computer Science at ETH Zurich, a member of Academia Europaea, and a Fellow of the ACM, IEEE, and ELLIS. He received the 2024 ACM Prize in Computing, one of the highest honors in the field. His research interests revolve around the central topic of "Performance-centric System Design" and include scalable networks, parallel programming techniques, and performance modeling. Torsten won best paper awards at the ACM/IEEE Supercomputing Conference SC10, SC13, SC14, SC19, SC22, SC23, SC24, HPDC'15, HPDC'16, IPDPS'15, and other conferences. He published hundreds of peer-reviewed scientific conference and journal articles and authored chapters of the MPI-2.2 and MPI-3.0 standards. He received the IEEE CS Sidney Fernbach Award, the ACM Gordon Bell Prize, the ISC Jack Dongarra award, the Latsis prize of ETH Zurich, as well as the German Max Planck-Humboldt Medal. Additional information about Torsten can be found on his homepage at htor.ethz.ch.



*Remaining program to be defined*



## Submissions

This is a traditional-style workshop without formal proceedings. 
The authors of accepted submissions will give a talk at the workshop and participate in the closing discussion panel. Additionally, authors will be invited to (optionally) upload their submitted paper (PDF) to be shared on the workshop website. 
A paper accepted to the HMEM workshop does not preclude its future publication at a major conference.

Submissions must use the [ACM proceedings template](https://www.acm.org/publications/proceedings-template) (for Latex users, version 1.90 (last update April 4, 2023) is the latest template, and please use the “sigconf” option). 

We accept two types of submissions.

A first type of submission includes position papers as well as papers that describe completed or early-stage work.
Such submissions are limited to 12 pages including references and figures.  
Extra pages can be included in a clearly marked appendix (to be read at the discretion of the reviewers).
Submitted papers must not include author names (double-blind review).

We also welcome 2-page abstracts that summarize recently accepted/published at top-tier conferences/journals. In this case, the author names and references to the published works should be included in the abstract.

Submit your paper here: [https://submissions.supercomputing.org](https://submissions.supercomputing.org)


## Important dates 

- Submission deadline: August 26th, 2025
- Notification of acceptance: September 15th, 2025
- Workshop: November 17th, 2025

Time Zone: AOE (Anywhere One Earth)


## Organization committee
- [Harald Servat](http://www.linkedin.com/in/harald-servat-7b543395), Intel
- [João Barreto](https://www.dpss.inesc-id.pt/~jpbarreto/), INESC-ID, Universidade de Lisboa
- [Antonio J. Peña](https://www.bsc.es/pena-antonio), Barcelona Supercomputing Center (BSC)

## Program committee

- Adrian Jackson, EPCC, UK
- Alexandro Baldassin, Universidade Estadual Paulista, Brasil
- Gokcen Kestor, PNNL, USA
- Dong Li, University of California, Merced, USA
- Gulay Yalcin, Abduallah Gul University, Turkey
- Ivy Peng, LLNL, USA
- Maciej Maciejewski, Huawei, Poland
- Marc Jordá, Barcelona Supercomputing Center, Spain
- Manolis Marazakis, Foundation for Research and Technology – Hellas (FORTH), GR
- Michael Hennecke,  Hewlett Packard Enterprise, Germany
- Swann Perarnau, Argonne National Laboratory (ANL), University of Chicago, USA
- Petar Radojkovic, Barcelona Supercomputing Center, Spain
- Tim Dykes, HPE, UK



## Previous editions

- [HMEM 2024](https://hmem-workshop.github.io/hmem2024/), colocated with CLUSTER'24

- [HMEM 2023](https://hmem-workshop.github.io/hmem2023/), colocated with SC'23

- [HMEM 2022](https://www.bsc.es/news/events/3rd-workshop-heterogeneous-memory-systems-hmem-2022), colocated with ICS'22

- [HMEM 2021](https://research-and-innovation.ec.europa.eu/events/upcoming-events/2nd-workshop-heterogeneous-memory-systems-hmem-2021-2021-06-18-0_en), colocated with ICS'21

- [HMEM 2020](https://research-and-innovation.ec.europa.eu/events/upcoming-events/1st-workshop-heterogeneous-memory-systems-hmem-2020-06-29_en/), colocated with ICS'20

