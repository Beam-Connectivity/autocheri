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

The performance-vs-security trade-off manifests different depending on the workload being processed by the system. A large part of the project is focussed on analysing, threat modelling and implementing four specific use cases. 

1. **Vehicle diagnostics data** - Processing data from CAN, through the TCU and up to the cloud.
1. **OTA software update** - Pulling software packages from the cloud, cryptographically verifying them, and passing on other vehicle ECUs.
1. **V2I traffic advisory** - Communicating with roadside infrastructure via cellular-V2X protocols.
1. **Teleoperation** - This is a use case that is safety critical and requires extremely low-latency, so is more impacted by poor performance.


### Consortium Partners

This project is made possible by the cross-sector collaboration of the consortium members:

1. **Applus IDIADA** - Systems engineering, validation and regulatory analysis
1. **Beam Connectivity** - Project lead, implementation and test of CHERI based telematics system
1. **CSA Catapult** - Industry stakeholder engagement and market analysis
1. **University of Exeter** - Software engineering support for CHERI
1. **Swansea University** - Cyber security analysis and threat modelling


# DSbD Technologies 

### What is CHERI?

CHERI stands for “Capability Hardware Enhanced RISC Instructions”. 

* Started in 2013, DARPA (US Defence Advanced Research Projects Agency) funded research by University of Cambridge.
* Over the last decade, many organisations have collaborated on CHERI including: Microsoft, Google and many universities.
* It is a new CPU instruction set architecture that offers two new features:
    * Enforces memory safety of pointers
    * Introduces ‘Capabilities’ to limit access to memory that was not expected by the original developers.

Read more about [CHERI from University of Cambridge](https://www.cl.cam.ac.uk/research/security/ctsrd/cheri)

### ... and Morello?

Morello is Arm's implementation of CHERI on Arm v8.2 architecture.
It is a development board, compiler & toolchain to allow us to write programs and run them leveraging CHERI

So for our project, Morello is the platform to prove the efficacy of CHERI in automotive domain.

Read more about [Arm's Morello Program](https://www.arm.com/architecture/cpu/morello    )


# News & Links

More to follow... 

* Beam Connectivity announce AutoCHERI kick-off - [https://www.beamconnectivity.com/blog/autocheri-project-announcement](https://www.beamconnectivity.com/blog/autocheri-project-announcement)
* Microsoft on CHERI - [https://msrc-blog.microsoft.com/2022/01/20/an_armful_of_cheris](https://msrc-blog.microsoft.com/2022/01/20/an_armful_of_cheris)
* UK Government announces AutoCHERI funding - [https://www.ukri.org/news/government-announces-new-national-cyber-strategy](https://www.ukri.org/news/government-announces-new-national-cyber-strategy)
