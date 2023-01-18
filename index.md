---
layout: default
---

Welcome! We are still at the start of the project, so this site will be updated as we progress... 


# What is the AutoCHERI🍒 project?

This project has three main goals:

1. Demonstrate CHERI technology for cyber critical and safety critical applications by: 
     developing a TCU based on Morello architecture for each use case, and
     Measure the security / safety / performance trade-offs and the impact of CHERI
1. Assess go-to-market routes for CHERI based products in automotive
1. Explore how this ties in with the emerging, global vehicle cyber security regulations

The performance-vs-security trade-off manifests differently depending on the workload being processed by the system. A large part of the project is focussed on analysing, threat modelling and implementing four specific use cases. 

1. **Vehicle diagnostics data** - Processing data from CAN, through the TCU and up to the cloud.
1. **OTA software update** - Pulling software packages from the cloud, cryptographically verifying them, and passing on other vehicle ECUs.
1. **V2I traffic advisory** - Communicating with roadside infrastructure via cellular-V2X protocols.
1. **Teleoperation** - This is a use case that is safety critical and requires extremely low-latency, so is more impacted by poor performance.


### Consortium Partners

This project is made possible by the cross-sector collaboration of the consortium members:

|:---:|:---:|:---:|:---:|:---:|
|![Applus-IDIADA](/assets/images/Applus+_IDIADA_Logo.png){: height="60" } | ![Beam-Connectivity](/assets/images/Beam Connectivity logo 900x300 transparent.png){: height="60" } | ![Beam-Connectivity](/assets/images/CSA-Catapult-transparent.png){: height="50" } | ![Beam-Connectivity](/assets/images/swansea-university-2017.en.png){: height="60" } | ![Beam-Connectivity](/assets/images/Uni_Exeter.svg.png){: height="60" }

* **Applus IDIADA** - Systems engineering, validation and regulatory analysis
* **Beam Connectivity** - Project lead, implementation and test of CHERI based telematics system
* **CSA Catapult** - Industry stakeholder engagement and market analysis
* **University of Exeter** - Software engineering support for CHERI
* **Swansea University** - Cyber security analysis and threat modelling



# DSbD Technologies 

### What is CHERI?

CHERI stands for **Capability Hardware Enhanced RISC Instructions**. CHERI extends conventional hardware Instruction-Set Architectures (ISAs) with new architectural features to enable fine-grained memory protection and highly scalable software compartmentalization. 

* Started in 2010, DARPA (US Defence Advanced Research Projects Agency) funded a joint research project of SRI International and the University of Cambridge.
* Over the last decade, many organisations have collaborated on CHERI including: Microsoft, Google and many universities.
* It is a new CPU instruction set architecture that offers two new features: 1) Enforces memory safety of pointers; 2) Introduces compartmentalisation.

**Memory-safe pointers**: The CHERI memory-protection features allow historically memory-unsafe programming languages such as C and C++ to be adapted to provide strong, compatible, and efficient protection against many currently widely exploited vulnerabilities. 

**Compartmentalization**: The CHERI scalable compartmentalization features enable the fine-grained decomposition of operating-system (OS) and application code, to limit the effects of security vulnerabilities in ways that are not supported by current architectures. 

Read more about [CHERI from University of Cambridge](https://www.cl.cam.ac.uk/research/security/ctsrd/cheri)

### ... and Morello?

Morello is Arm's implementation of CHERI on Arm v8.2 architecture.
It is a development board, compiler & toolchain to allow us to write programs and run them leveraging CHERI

So for our project, Morello is the platform to prove the efficacy of CHERI in automotive domain.

Read more about [Arm's Morello Program](https://www.arm.com/architecture/cpu/morello    )

# Find out more

### Presentations

* DSbD All Hands, October 2022 - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/DSbD+All+Hands+Oct+2022+-+AutoCHERI+update.pdf)
* Lesson from Integrating Morello into vehicle systems - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/Beam+Connectivity+-+Lessons+from+Integrating+Morello+into+Vehicle+System.pdf), Webcast video (coming soon!)


### News & Links

* Beam Connectivity announce AutoCHERI kick-off - [https://www.beamconnectivity.com/blog/autocheri-project-announcement](https://www.beamconnectivity.com/blog/autocheri-project-announcement)
* Microsoft on CHERI - [https://msrc-blog.microsoft.com/2022/01/20/an_armful_of_cheris](https://msrc-blog.microsoft.com/2022/01/20/an_armful_of_cheris)
* UK Government announces AutoCHERI funding - [https://www.ukri.org/news/government-announces-new-national-cyber-strategy](https://www.ukri.org/news/government-announces-new-national-cyber-strategy)
