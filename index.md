# 7th Workshop on Heterogeneity and Memory Systems (HMEM 2026)

### In conjunction with [SC'26](https://sc26.supercomputing.org/), Chicago, IL, November 16th, 2026


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

# November 16th, 2026

### 14:00 Welcome 

### 14:00-15:00 Hotness tracking in CXL hardware

**Featured speaker: Yan Sun,** University of Illinois at Urbana-Champaign, USA

*Abstract: 
Growing application memory demands are motivating heterogeneous memory systems that combine local DRAM with CXL-attached capacity. Their performance depends on identifying which data should occupy the faster tier and adapting placement as access patterns change. M5 and ARC are two complementary approaches to hardware–software co-design for CXL memory management. M5 uses device-side page and subpage tracking to guide migration, while ARC adapts the counting organization to workload behavior using shared hardware storage. Through measurements on real CXL prototypes, we examine how the location, granularity, and organization of hotness tracking influence migration decisions and application performance, highlighting trade-offs and opportunities for coordinating memory monitoring and placement.* 

*Bio:
Yan Sun is a Ph.D. candidate in Electrical and Computer Engineering at the University of Illinois Urbana-Champaign, advised by Professor Nam Sung Kim. Yan’s research focuses on hardware–software co-design for memory and datacenter systems, particularly CXL-based memory architectures and management. His work spans memory characterization, tiering, and near-memory processing, with publications at MICRO, ASPLOS, OSDI, SOSP, and USENIX ATC.*

### 15:00-15:30 Coffee break

### 15:30-17:30 Accepted papers

**Optimizing system memory bandwidth with micron CXL memory expansion modules on intel Xeon 6 processors**, 
Anil Godbole [\*], Rohit Sehgal, Vinicius Petrucci and Vishal Tanna, Intel Corporation [\*] and Micron, USA

*Abstract: High-Performance Computing (HPC) and Artificial Intelligence (AI) workloads typically demand substantial memory bandwidth and, to a degree, memory capacity. CXL memory expansion modules, also known as CXL "type-3" devices, enable enhancements in both memory capacity and bandwidth for server systems by utilizing the CXL protocol which runs over the PCIe interfaces of the processor. This paper discusses experimental findings on achieving increased memory bandwidth for HPC and AI workloads using Micron's CXL modules. Memory expansion via CXL boosts read-only bandwidth by 24% and mixed read/write bandwidth by up to 39%. Across HPC and AI workloads, the geometric mean of performance speedups is 24%.*

**One API, Five Memories: Measuring Unified Memory Across NVIDIA and AMD Architectures**, 
Alexandre Bardakoff, Adrien Roussel [\*] and Kento Sato, RIKEN Center for Computational Science (R-CCS), Japan, and CEA, France [\*].

*Abstract: Managed memory promises one pointer that both the CPU and the GPU can dereference, with the system deciding where the pages live. We measured what that promise means on five systems: NVIDIA H100 NVL, GH200, GB10, and AMD MI300A and MI300X, running one benchmark identically on all of them: a page-granular pointer chase bracketed by device- and host-resident anchor buffers, cross-checked by an operating-system residency probe, and probing placement, lifecycle costs, memory pressure, memAdvise hints, and concurrency. The five systems follow four different placement rules. The same managed access costs 244ns on an empty H100 and 40152ns when GPU memory is full; the GH200 degrades eightfold under the same pressure, the GB10 not at all. Hints rescue the H100 by 40x, harm the GH200 by up to 44x and are inert on single-pool systems. A routine operating-system update rewrote the MI300X's placement rule on unchanged hardware and ROCm.*

**Extending ecoHMEM to Arm: Automatic Data Placement Using Statistical Profiling Extension**, 
Marc Jordà and Antonio J. Peña, Barcelona Supercomputing Center (BSC), Spain.

*Abstract: The growing diversification of high-performance processor architectures and adoption of heterogeneous memory systems introduce new challenges for performance portability and efficient memory management. As Arm-based platforms gain relevance in HPC and technologies such as HBM and CXL memory expansion become widespread, mechanisms that automatically exploit memory heterogeneity are increasingly important. Precise sampled hardware events have proven valuable for characterizing memory behavior across processor families, but their use on Arm has only recently become feasible with the Statistical Profiling Extension (SPE). In this work, we extend the ecoHMEM automatic data-placement framework to Arm-based systems by leveraging SPE to obtain precise memory-access information. We design and implement the required profiling infrastructure and analyze its key tradeoffs. Experimental evaluation on an Arm system with emulated memory heterogeneity demonstrates the feasibility of integrating SPE into automatic data placement, achieving performance improvements of up to 22% over mainstream NUMA strategies.*

**An ELF-Aware DMA Engine for Distributed-Memory Accelerators**, 
Jaskin Kabir and Ron Sass, North Carolina State University and University of North Carolina at Charlotte, USA.

*Abstract: Distributed-memory, many-core accelerators are often bottlenecked by the task of transferring data to and from the local memories. Existing solutions place much of the orchestration burden onto the host processor. Instead, we propose an ELF-aware DMA engine that parses an ELF file from host memory and uses off-the-shelf DMA and interconnect IP to transfer data with minimal host intervention. We also extend the ELF format to encode both high-fan-out load and many-to-one gather operations in one file. On our FPGA proxy modeled after a kilocore accelerator, our design is 4.8× faster than host memcpy and 39% faster than scatter-gather DMA on load, with host preprocessing reduced to two register writes. Extrapolation to the kilocore scale suggests the engine costs roughly 1.6% of PE capacity. For many-core distributed-memory accelerators, we conclude that this approach is a viable middle ground between the host manually transferring bytes and a custom NoC/DMA stack.*


## Submissions

This is a traditional-style workshop without formal proceedings. 
The authors of accepted submissions will give a talk at the workshop and participate in the closing discussion panel. Additionally, authors will be invited to (optionally) upload their submitted paper (PDF) to be shared on the workshop website. 
A paper accepted to the HMEM workshop does not preclude its future publication at a major conference.

Submissions must use the [IEEE proceedings template](https://www.ieee.org/conferences/publishing/templates), two-column page format.

We accept two types of submissions.

A first type of submission includes position papers as well as papers that describe completed or early-stage work. Such submissions are limited to 10 pages including references and figures, but excluding bibliography.
Submitted papers must not include author names (double-blind review).

We also welcome 2-page abstracts that summarize recently accepted/published at top-tier conferences/journals. In this case, the author names and references to the published works should be included in the abstract.

Submit your paper here: [https://submissions.supercomputing.org](https://submissions.supercomputing.org)


## Important dates 

- Submission deadline: **August 31, 2026 (extended)**
- Notification of acceptance: September 15, 2026
- Workshop: November 16th, 2026

Time Zone: AOE (Anywhere One Earth)


## Organization committee
- [Harald Servat](http://www.linkedin.com/in/harald-servat-7b543395), Intel
- [João Barreto](https://www.dpss.inesc-id.pt/~jpbarreto/), INESC-ID, Universidade de Lisboa
- [Antonio J. Peña](https://www.bsc.es/pena-antonio), Barcelona Supercomputing Center (BSC)

## Program committee

- Adrian Jackson, University of Edinburgh, UK
- Alexandro Baldassin, UNESP, Brazil
- Brice Videau, Argonne National Laboratory, USA
- Chloe Alverti, National Technical University of Athens, Greece
- Clément Foyer, Université de Reims Champagne-Ardenne, France
- Dong Li, University of California, Merced, USA
- Gulay Yalçin, Ankara Yildirim Beyazit University, Turkey
- Maciej Maciejewski, Huwaei, Poland
- Manolis Marazakis, Foundation for Research and Technology – Hellas (FORTH), Greece
- Marc Jorda, Barcelona Supercomputing Center (BSC), Spain
- Petar Radojkovic, Barcelona Supercomputing Center (BSC); Polytechnic University of Catalonia, Spain
- Sudharshan S. Vazhkudai, Micron Technology Inc, USA
- Swann Perarnau, Argonne National Laboratory (ANL), University of Chicago, USA
- Tim Dykes, Hewlett Packard Enterprise (HPE), UK





## Previous editions

- [HMEM 2025](https://hmem-workshop.github.io/hmem2025/), colocated with SC'25

- [HMEM 2024](https://hmem-workshop.github.io/hmem2024/), colocated with CLUSTER'24

- [HMEM 2023](https://hmem-workshop.github.io/hmem2023/), colocated with SC'23

- [HMEM 2022](https://www.bsc.es/news/events/3rd-workshop-heterogeneous-memory-systems-hmem-2022), colocated with ICS'22

- [HMEM 2021](https://research-and-innovation.ec.europa.eu/events/upcoming-events/2nd-workshop-heterogeneous-memory-systems-hmem-2021-2021-06-18-0_en), colocated with ICS'21

- [HMEM 2020](https://research-and-innovation.ec.europa.eu/events/upcoming-events/1st-workshop-heterogeneous-memory-systems-hmem-2020-06-29_en/), colocated with ICS'20

