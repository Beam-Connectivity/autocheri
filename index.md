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
|![Beam-Connectivity](/assets/images/Beam Connectivity logo 900x300 transparent.png){: height="60" } | ![Applus-IDIADA](/assets/images/Applus+_IDIADA_Logo.png){: height="60" }  | ![Beam-Connectivity](/assets/images/CSA-Catapult-transparent.png){: height="50" } | ![Beam-Connectivity](/assets/images/swansea-university-2017.en.png){: height="60" } | ![Beam-Connectivity](/assets/images/Uni_Exeter.svg.png){: height="60" }

* **Beam Connectivity** - Project lead, implementation and test of CHERI based telematics system
* **Applus IDIADA** - Systems engineering, validation and regulatory analysis
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
* 06/09/2023 - Cenex-CAM Conference - Secure hardware for connected vehicles - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/AutoCHERI%20-%20Cenex-LCV%20-%20Sept%202023.pdf)
* 10/05/2023 - GAAC Presentation on Cyber Security Challenges For Connected Vehicles - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/SEMI-GAAC-BeamConnectivity-connected-security-PUBLIC.pdf)
* 17/01/2023 - Lesson from Integrating Morello into vehicle systems - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/Beam+Connectivity+-+Lessons+from+Integrating+Morello+into+Vehicle+System.pdf), [Webcast video](https://www.youtube.com/watch?v=u58BDmhonSE)
* 13/10/2022 - DSbD All Hands, October 2022 - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/DSbD+All+Hands+Oct+2022+-+AutoCHERI+update.pdf)


### News & Links

* 31/04/2023 - CISA Paper on Digital Security by Design (DSbD) mentioning CHERI - [https://www.cisa.gov/resources-tools/resources/secure-by-design-and-default](https://www.cisa.gov/resources-tools/resources/secure-by-design-and-default)
* 06/02/2023 - Microsoft implementing CHERI on RISC-V - [https://www.microsoft.com/en-us/research/publication/cheriot-rethinking-security-for-low-cost-embedded-systems/](https://www.microsoft.com/en-us/research/publication/cheriot-rethinking-security-for-low-cost-embedded-systems/)
* 21/11/2022 - Protecting OpenSSL with CHERI, from NquiringMinds - [https://manysecured.net/openssl/](https://manysecured.net/openssl/)
* 19/07/2022 - Beam Connectivity announce AutoCHERI kick-off - [https://www.beamconnectivity.com/blog/autocheri-project-announcement](https://www.beamconnectivity.com/blog/autocheri-project-announcement)
* 20/10/2022 - Microsoft on CHERI - [https://msrc.microsoft.com/blog/2022/01/an_armful_of_cheris/](https://msrc.microsoft.com/blog/2022/01/an_armful_of_cheris/)
* 15/12/2021 - UK Government announces AutoCHERI funding - [https://www.ukri.org/news/government-announces-new-national-cyber-strategy](https://www.ukri.org/news/government-announces-new-national-cyber-strategy)
