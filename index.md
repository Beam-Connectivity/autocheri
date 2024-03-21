---
layout: default
---

Cyber security is of critical importance to the automotive industry, as the volume and complexity of hacks is increasing. Securing Connected and Autonomous Vehicles (CAVs) is a particular challenge as they expose a multitude of wireless interfaces and process data from untrusted, external systems via: cellular, GPS, Wi-Fi/BT, C-V2X, camera and sensor inputs.

The AutoCHERI🍒 project is focussed on the area of CAV cyber security and the opportunities and challenges that CHERI might bring in this sector.

- - -

This project site covers:
* [Project Summary](#project-summary)
* [What is CHERI?](#dsbd-technologies)
* [Find out more](#find-out-more)
* [Automotive Security by Design Summit: Coventry, UK](#automotive-security-by-design-summit-uk)
* [Automotive Security by Design Summit: Munich, Germany](#automotive-security-by-design-summit-munich)

- - -

# Project Summary

This project has three main goals:

1. Demonstrate CHERI technology for cyber critical and safety critical applications by: 
<br/>- Developing a TCU based on Morello architecture for each use case, and
<br/>- Measure the security / safety / performance trade-offs and the impact of CHERI
1. Assess go-to-market routes for CHERI based products in the automotive industry
1. Explore how this ties in with the emerging, global vehicle cyber security regulations

The performance-vs-security trade-off manifests differently depending on the workload being processed by the system. 

A large part of the project is focussed on analysing, threat modelling and implementing a number of specific use cases. With these specific workloads, we can then compare the performance impact of enabling CHERI capabilities and understand if what types of workload CHERI might be more or less appropriate for. The use cases that are being evaluated: 

1. **Vehicle diagnostics data** - Processing data from CAN, through the TCU and up to the cloud.
1. **OTA software update of TCU** - Pulling software packages from the cloud, cryptographically verifying them.
1. **V2I traffic advisory** - Communicating with roadside infrastructure via cellular-V2X protocols.
1. **Teleoperation** - Monitoring latency in safety critical operations to observe where additional processing would cause an impact.
1. **OTA software update of RISC-V vehicle ECUs** - For a RISC-V CHERI ECU, pulling software packages from the cloud and updating them over CAN using UDS. 

### Consortium Partners

This project is made possible by the cross-sector collaboration of the consortium members:

|:---:|:---:|:---:|:---:|:---:|
|![Beam-Connectivity](/assets/images/Beam Connectivity logo 900x300 transparent.png){: height="60" } | ![Applus-IDIADA](/assets/images/Applus+_IDIADA_Logo.png){: height="60" }  | ![Beam-Connectivity](/assets/images/CSA-Catapult-transparent.png){: height="50" } | ![Beam-Connectivity](/assets/images/swansea-university-2017.en.png){: height="60" } | ![Beam-Connectivity](/assets/images/University of Exeter_Crest_Logo_RGB_Uni_Landscape_Pos_Lrg.png){: height="60" }

* **Beam Connectivity** - Project lead, implementation and integration of CHERI based automotive component
* **Applus IDIADA** - Systems engineering, validation and regulatory analysis
* **CSA Catapult** - Industry stakeholder engagement and market analysis
* **University of Exeter** - Software engineering support for CHERI
* **Swansea University** - Cyber security analysis and threat modelling

- - - 

# DSbD Technologies 

### What is CHERI?

CHERI stands for **Capability Hardware Enhanced RISC Instructions**. CHERI extends conventional hardware Instruction-Set Architectures (ISAs) with new architectural features to enable fine-grained memory protection and highly scalable software compartmentalization. 

* Started in 2010, DARPA (US Defence Advanced Research Projects Agency) funded a joint research project of SRI International and the University of Cambridge.
* Over the last decade, many organisations have collaborated on CHERI including: Microsoft, Google and many universities.
* It is a new CPU instruction set architecture that offers two new features: 1) Enforces memory safety of pointers; 2) Introduces compartmentalisation.

**Memory-safe pointers**: The CHERI memory-protection features allow historically memory-unsafe programming languages such as C and C++ to be adapted to provide strong, compatible, and efficient protection against many currently widely exploited vulnerabilities. 

**Compartmentalization**: The CHERI scalable compartmentalization features enable the fine-grained decomposition of operating-system (OS) and application code, to limit the effects of security vulnerabilities in ways that are not supported by current architectures. 

Read more about [CHERI from University of Cambridge](https://www.cl.cam.ac.uk/research/security/ctsrd/cheri)

### The Morello prototyping platform

Morello is Arm's implementation of CHERI on Arm v8.2 architecture.
It is a development board, compiler & toolchain to allow us to write programs and run them leveraging CHERI

So for our project, Morello is the platform to prove the efficacy of CHERI in the automotive domain.

Read more about [Arm's Morello Program](https://www.arm.com/architecture/cpu/morello    )

### CHERI-Enabled RISC-V

An extension of RISC-V to support CHERI-based capabilities [(CHERI-RISC-V)](https://www.cl.cam.ac.uk/research/security/ctsrd/cheri/cheri-risc-v.html) has been developed, providing an open-source alternative to Morello. 

This provides exciting opportunities for companies to begin prototyping and commercializing CHERI technology, and some companies such as [Codasip](https://codasip.com/solutions/riscv-processor-safety-security/cheri/) have made commercial CHERI-enabled RISC-V processors available. 

- - -

# Find out more
### AutoCHERI Project Showcase
Watch the video we created to explain the work we've done. Includes perspectives from our project partners on why our work is impactful, and footage from our on-track testing. 

[https://www.youtube.com/watch?v=dwkpQC-laIU](https://www.youtube.com/watch?v=dwkpQC-laIU)

### Presentations

* 01/02/2024 - AutoCHERI Summit, February 2024 - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/AutoCHERI%20Workshop%20240201.pdf)
* 17/01/2023 - Lesson from Integrating Morello into vehicle systems - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/Beam+Connectivity+-+Lessons+from+Integrating+Morello+into+Vehicle+System.pdf), [Webcast video](https://www.youtube.com/watch?v=u58BDmhonSE)
* 13/10/2022 - DSbD All Hands, October 2022 - [PDF slides](https://beam-infra-public-bucket-s3bucket-w7tdylcrnx9g.s3.eu-west-1.amazonaws.com/blog-assets/DSbD+All+Hands+Oct+2022+-+AutoCHERI+update.pdf)


### News & Links

* 30/01/2024 - Infosecurity Europe article on Digital Security By Design - [https://www.infosecurityeurope.com/en-gb/blog/future-thinking/dsbd-vulnerability-management-cycle.html](https://www.infosecurityeurope.com/en-gb/blog/future-thinking/dsbd-vulnerability-management-cycle.html)
* 31/04/2023 - CISA Paper on Digital Security by Design (DSbD) mentioning CHERI - [https://www.cisa.gov/resources-tools/resources/secure-by-design-and-default](https://www.cisa.gov/resources-tools/resources/secure-by-design-and-default)
* 06/02/2023 - Microsoft implementing CHERI on RISC-V - [https://www.microsoft.com/en-us/research/publication/cheriot-rethinking-security-for-low-cost-embedded-systems/](https://www.microsoft.com/en-us/research/publication/cheriot-rethinking-security-for-low-cost-embedded-systems/)
* 21/11/2022 - Protecting OpenSSL with CHERI, from NquiringMinds - [https://manysecured.net/openssl/](https://manysecured.net/openssl/)
* 19/07/2022 - Beam Connectivity announce AutoCHERI kick-off - [https://www.beamconnectivity.com/blog/autocheri-project-announcement](https://www.beamconnectivity.com/blog/autocheri-project-announcement)
* 20/10/2022 - Microsoft on CHERI - [https://msrc.microsoft.com/blog/2022/01/an_armful_of_cheris/](https://msrc.microsoft.com/blog/2022/01/an_armful_of_cheris/)
* 15/12/2021 - UK Government announces AutoCHERI funding - [https://www.ukri.org/news/government-announces-new-national-cyber-strategy](https://www.ukri.org/news/government-announces-new-national-cyber-strategy)

- - - 

# Automotive Security by Design Summit, UK

The AutoCHERI consortium hosted a workshop on 01 February 2024 to bring together leaders in automotive cyber security to discuss the challenges the industry is facing. With a focus on taking a holistic, security by design approach, the delegates explored the value that secure hardware foundations can bring to the automotive industry.

Summit delegates included experts from a number of sectors including: Tier 1s, automotive OEMs, academia, semiconductor design, and cyber security.

![Beam-Connectivity](/assets/asbd-workshop/banner-image2.png){: width="900" 
style="display: block; margin: 0 auto}| !

### Presentations and Demos

The presentations included:

1. **Cybersecurity and Resilience in Automotive Hardware: The Challenges Ahead** - *Paul Wooderson, Chief Engineer, Cybersecurity, HORIBA MIRA*
1. **Automotive Cyber Security: From a Connectivity Viewpoint** - *Thomas Sors, CEO, Beam Connectivity*
1. **Enhanced Hardware Silver Bullet or Lead Weight and why it matters whether you are werewolf or fish** - *Peter Davies, Technical Director, THALES*
1. **AESIN: The UK Automotive Electronics Systems Innovation Network** - *Gunny Ghadyalla, Director, AESIN*

![Beam-Connectivity](/assets/asbd-workshop/presentation-from-back.jpeg){: width="900" style="display: block; margin: 0 auto"} 


### Workshop

The workshop was focussed on cyber security challenges introduced by a supply chain complexity and the evolving vehicle architectures - setting our time horizon to 5+ years in the future.

The workshop sessions considered three specific questions:

1. As vehicle platforms evolve towards more consolidated compute hardware, how can cyber-critical & performance-sensitive processes be isolated from each other? 
1. As software content increases & software supply chain becomes more complex, how can the quality & security of all the dependencies be ensured to prevent huge loss and damage in years to come?
1. There are numerous areas of cyber resilience that need attention in the automotive industry. What are the major challenge areas?


There were also demonstrations from AutoCHERI and ResAuto innovation projects showed how advanced hardware security might be applied.

![Beam-Connectivity](/assets/asbd-workshop/vehicle-demo-cameron-outside-1.jpeg){: height="280"}
![Beam-Connectivity](/assets/asbd-workshop/workshop-session-from-back.jpg){: height="280"}


# Automotive Security by Design Summit, Munich

📣 The next event hosted by the AutoCHERI consortium will take place in Munich on the 6th May 2024. 

For further details about the event or to register your attendence, please click see the eventbrite page:

[https://www.eventbrite.co.uk/e/automotive-security-by-design-workshop-munich-tickets-849514098537](https://www.eventbrite.co.uk/e/automotive-security-by-design-workshop-munich-tickets-849514098537)


![Beam-Connectivity](/assets/asbd-workshop-munich/Blue%20Neon%20Welcome%20To%20Our%20Gallery%20Email%20Header%20(8).png){: width="900" 
style="display: block; margin: 0 auto}| !