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

### November 17th, 2025

### 14:00 Welcome 

### 14:00-15:00 Featured talk: **ARMing GPUs: On the Memory Subsystem of Grace Hopper GH200**, Torsten Hoefler, ETH Zurich, Switzerland



*Abstract: Heterogeneous supercomputers have become the standard in HPC. GPUs in particular have dominated the accelerator landscape, offering unprecedented performance in parallel workloads and unlocking new possibilities in fields like AI and climate modeling. With many workloads becoming memory-bound, improving the communication latency and bandwidth within the system has become a main driver in the development of new architectures. The Grace Hopper Superchip (GH200) is a significant step in the direction of tightly coupled heterogeneous systems, in which all CPUs and GPUs share a unified address space and support transparent fine grained access to all main memory on the system. We characterize both intra- and inter-node memory operations on the Quad GH200 nodes of the new Swiss National Supercomputing Centre Alps supercomputer, and show the importance of careful memory placement on example workloads, highlighting tradeoffs and opportunities.* 

*Bio: Torsten Hoefler is a Professor of Computer Science at ETH Zurich, a member of Academia Europaea, and a Fellow of the ACM, IEEE, and ELLIS. He received the 2024 ACM Prize in Computing, one of the highest honors in the field. His research interests revolve around the central topic of "Performance-centric System Design" and include scalable networks, parallel programming techniques, and performance modeling. Torsten won best paper awards at the ACM/IEEE Supercomputing Conference SC10, SC13, SC14, SC19, SC22, SC23, SC24, HPDC'15, HPDC'16, IPDPS'15, and other conferences. He published hundreds of peer-reviewed scientific conference and journal articles and authored chapters of the MPI-2.2 and MPI-3.0 standards. He received the IEEE CS Sidney Fernbach Award, the ACM Gordon Bell Prize, the ISC Jack Dongarra award, the Latsis prize of ETH Zurich, as well as the German Max Planck-Humboldt Medal. Additional information about Torsten can be found on his homepage at htor.ethz.ch.*


### 15:00-15:30 Coffee break

### 15:30-17:00 Accepted papers

**Machine Learning-Guided Memory Optimization for DLRM Inference on Tiered Memory**, 
Bin Ma, Jie Ren, Shuangyan Yang and Dong Li, University of California, Merced, USA

*Abstract: Deep learning recommendation models (DLRMs) rely on massive embedding tables that often exceed GPU memory capacity. Tiered memory offers a cost-effective solution but creates challenges for managing irregular access patterns. We introduce RecMG, an ML-guided caching and prefetching system tailored for DLRM inference. RecMG uses separate models for short-term reuse and long-range prediction, with a novel differentiable loss to improve accuracy. In large-scale deployments, RecMG reduces on-demand fetches by up to 2.8× and cuts inference time by up to 43%.*

**Performance Analysis of Compute Express Link (CXL) Memory Expansion with Data Interleaving**, Tung-Yu Hsieh and Jerry Chou, National Tsing Hua University, Taiwan

*Abstract: The performance gap between processors and memory has become a significant bottleneck nowadays, commonly referred to as the Memory Wall. Compute Express Link emerges as a promising solution to address these challenges by providing benefits to expand the memory space and bandwidth. In this work, we focus on the performance measurement and analysis of the memory interleaving strategy on CXL memory. Our experiments, conducted on both simulated and genuine CXL-enabled system, show that the naive interleaving configurations cannot always deliver the best memory bandwidth. In fact, it could be 26.97% less than the optimal configuration in the worst case. Besides, we observed distinct characteristics between emulated and genuine CXL system, presenting the limitation of evaluating performance by simulation for memory interleaving. Our work reveals the importance of interleaving configurations and provide the performance comparison with analyses for identifying the influencing factors and developing guideline of the CXL memory placement policy.*

**A Limits Study of Memory-side Tiering Telemetry**, Vinicius Petrucci, Felippe Zacarias and David Roberts, Micron Technology, USA

*Abstract: Increasing workload demands and emerging technologies necessitate the use of various memory and storage tiers in computing systems. This paper presents results from a CXL-based Experimental Memory Request Logger that reveals precise memory access patterns at runtime without interfering with the running workloads. By combining reactive placement based on data address monitoring, proactive data movement, and compiler hints, a Hotness Monitoring Unit (HMU) within memory modules can greatly improve memory tiering solutions. Analysis of page placement using profiled access counts on a Deep Learning Recommendation Model (DLRM) indicates a potential 1.94x speedup over Linux NUMA balancing tiering, and only a 3% slowdown compared to Host-DRAM allocation while offloading over 90% of pages to CXL memory. The study underscores the limitations of existing tiering strategies in terms of coverage and accuracy, and makes a strong case for programmable, device-level telemetry as a scalable and efficient solution for future memory systems.*

**Summary: Hierarchical Framework for Multi-node Compute eXpress Link Memory Transactions**, Ellis Giles (Coda Solutions) and Peter Varman (Rice University), USA

*Abstract: There is a growing need to support high-volume, concurrent transaction processing on shared data in both high-performance computing and data center environments. A recent innovation in server architectures is the use of disaggregated memory organizations based on the Compute eXpress Link (CXL) interconnect protocol. While CXL memory architectures alleviate many concerns in data centers, enforcing ACID semantics for transactions in CXL memory faces many challenges. This paper is a summary of a full paper at MEMSYS25, where we describe a novel solution for supporting ACID (Atomicity, Consistency, Isolation, Durability) transactions in a CXL-based disaggregated shared-memory architecture. We call this solution HTCXL for Hierarchical Transactional CXL. HTCXL is implemented in a software library that enforces transaction semantics within a host, along with a back-end controller to detect conflicts across hosts. HTCXL is a modular solution allowing different combinations of HTM or software-based transaction management to be mixed as needed.*

**Performance Characterization of CXL Memory and Its Use Cases**, Xi Wang (University of California, Merced), Jie Ren (William & Mary) and Dong Li (University of California, Merced), USA

*Abstract: Compute eXpress Link (CXL) is emerging as a promising memory interface technology. However, its performance characteristics remain largely unclear due to the limited availability of production hardware. In this work, we study how HPC applications and large language models (LLM) can benefit from the CXL memory, and study the interplay between memory tiering and page interleaving. We also propose a novel data object-level interleaving policy to match the interleaving policy with memory access patterns. Our findings reveal the challenges and opportunities of using CXL.*

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

- Submission deadline: **September 1, 2025 (extended)**
- Notification of acceptance: September 15, 2025
- Workshop: November 17, 2025

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

