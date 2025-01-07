---
title: Background
nav_order: 1
layout: home
permalink: "/"
lang: en
---

# Focus on making great missions
{: .no_toc }
Build-A-Satellite gives your satellite development team a jumpstart with robust documentation tailored to the customizable BIRDS cube satellite bus, referencing susbsystem specific respositories hosted on GitHub.

[Get Started Now]({{site.url}}/get-started){: .btn .btn-purple }

<details markdown="block">
<summary>Table of Contents</summary>

- Table of Contents
{:toc}

</details>

# *Background*
{: .no_toc }

## **1. Introduction**
  
   This guide is intended to facilitate a comprehensive understanding of the usage of BIRDS Bus subsystem testing documents, empowering team members and collaborators to follow standardized procedures for reliable subsystem performance. 

   This document outlines the purpose, structure, and practical steps for using the testing process and procedural guides for subsystems such as the 
   - On-Board Computer (OBC), 
   - Electrical Power System (EPS), 
   - Attitude Determination and Control System (ADCS), 
   - Communications (COM), 
   - and the structural components of BIRDS satellites.

### We are creating an environment for sharing knowledge and ideas.
{: .no_toc }
To help you create your own open source satellite mission, we are building a library of resources that will cover the entire mission lifetime from start to finish. 

If you would want to contribute to, or work with the [BIRDS] community in order to assist in developing this solution, please contibute to the [our Discussions channel on Github] or [get in touch with us.]

## **2. What are the phases of a satellite?**
  The development and deployment of a satellite involve a series of carefully structured phases to ensure the mission's success. From initial concept discussions to final pre-launch verifications, these phases guide teams through designing, building, and testing the satellite to meet stringent space industry standards. 
    
  Each phase acts as a checkpoint to confirm that requirements are met and potential risks are mitigated. Understanding the phases - including the
  - Mission Definition Review (MDR), 
  - Preliminary Design Review (PDR), 
  - Critical Design Review (CDR), and 
  - Flight Readiness Review (FRR) 


```mermaid
gantt
    title Satellite Milestones
    dateFormat  YYYY-MM-DD
    section  Mission concept 
    MDR     :milestone, crit, a2, 2014-01-23, 4d
    A task  :crit, done, a1, 2014-01-20, 9d
    section Bus + Payload dev. & testing
    PDR      :milestone, crit, a3, 2014-02-3, 4d
    another task    :active, 2014-01-20  , 31d
    section EM integration & testing
    CDR     :milestone, crit, 2014-02-20, 4d
    another task      : 2014-02-12  , 12d
    section Software dev.
    FM     :milestone, crit, 2014-03-09, 4d
    another task      :active, 2014-02-03  , 38d
    section FM integration & testing
    another task      :2014-02-26  , 15d
    section GS software revision
    another task      :after a3, 30d
    section End-to-End test
    another task      : 2014-03-01, 13d
    section Operation plan 
    another task      : 2014-03-04, 12d
    section Freq. coord. IARU
    another task      : crit, active, after a2, 53d
    section Satellite delivery
    another task      : 2014-03-16,12d
    section Launch
    another task      : 5d
    section Operation
    another task      : 10d
    section Disposal
```


### *Mission Definition Review (MDR)*
- The Mission Definition Review is the initial phase where the primary objectives and feasibility of the satellite mission are assessed. It ensures that the mission concept aligns with stakeholder goals and meets basic feasibility criteria.
- **Key Activities**:
  - **Requirements Definition**: Establishing the mission's main objectives, such as scientific data collection, Earth observation, or communication.
  - **Concept Analysis**: Evaluating different mission concepts and selecting the most viable one.
  - **Preliminary Budgeting**: Outlining initial cost estimates and resource needs.
  - **Risk Assessment**: Identifying potential high-level risks and challenges.
- **Outcome**: Approval to proceed to the design phase. The outcome of the MDR is a clearly defined mission scope with initial high-level requirements.

### *Preliminary Design Review (PDR)*
- The Preliminary Design Review is a crucial checkpoint to assess whether the preliminary design of the satellite meets the mission's requirements and objectives. It ensures that the basic design approach is sound before advancing to more detailed design work.
- **Key Activities**:
  - **Subsystem Design Overview**: Presenting initial design plans for key subsystems like OBC, EPS, ADCS, COM, payloads, and structure.
  - **Preliminary Schematics**: Showing preliminary circuit diagrams, mechanical layouts, and software architecture.
  - **Interface Definition**: Outlining how different subsystems will interact and integrate.
  - **Verification Plan**: Drafting a plan for how each requirement will be tested and verified in later phases.
- **Outcome**: Approval to move to detailed design and further development. If the PDR is successful, the project team receives a green light to refine and deepen their designs.

### *Critical Design Review (CDR)*
- The Critical Design Review is an in-depth evaluation of the final design before it transitions into production and assembly. The aim is to verify that the detailed design meets all mission requirements and is manufacturable and testable.
- **Key Activities**:
  - **Detailed Design Presentation**: Showcasing detailed drawings, CAD models, circuit layouts, and software implementation.
  - **Compliance Check**: Ensuring that the design adheres to industry standards, regulatory requirements, and internal specifications.
  - **Risk Mitigation Plans**: Reviewing the updated risk register and contingency plans.
  - **Manufacturing Readiness**: Assessing the readiness of production facilities, supply chains, and assembly processes.
- **Outcome**: Approval to proceed to the manufacturing and integration phase. A successful CDR means that the design is considered final, and the team can start producing and assembling components.

### *Flight Readiness Review (FRR)*
- Flight Model Testing is the phase where the actual satellite, known as the Flight Model (FM), undergoes a series of rigorous tests to validate its performance under conditions that simulate the space environment. This is the final verification before launch.
- **Key Activities**:
  - **Functional Testing**: Verifying that each subsystem and the satellite as a whole function as expected.
  - **Environmental Testing**:
    - **Thermal Vacuum (TVT) Testing**: Ensuring the satellite can withstand the extreme temperatures and vacuum conditions of space.
    - **Vibration Testing**: Testing for structural integrity under launch conditions to ensure it can survive the launch vibrations.
  - **Deployment Testing**: Verifying the proper deployment of antennas, solar panels, or other movable parts.
- **Outcome**: Confirmation that the satellite is ready for launch. Any failures during this phase may require redesign, rework, or additional testing until issues are resolved and the satellite meets all operational standards.

### *Conclusion*
{: .no_toc }
These phases create a structured pathway from conceptualization to launch, with each review and testing stage serving as a critical checkpoint. The **Mission Definition Review** sets the scope, the **Preliminary Design Review** checks the initial design feasibility, the **Critical Design Review** finalizes the detailed design, and **Flight Model Testing** ensures that the satellite is robust and mission-ready. This structured approach helps in mitigating risks, ensuring quality, and promoting mission success.

## **3. What is in the BIRDS bus?**
<p>
  <img alt="birdsx-frame" src="assets/images/birdsx-ext-assembly.png" width="45%">
&nbsp;
  <img alt="birdsx-board-frame" src="assets/images/birdsx-board-layout.png" width="45%">
</p>

The bus includes the following key components:

**On-Board Computer (OBC)**: Handles the satellite’s core computing needs.

**Electrical Power System (EPS)**: Manages power generation, storage, and distribution.

**Attitude Determination and Control System (ADCS)**: Controls satellite orientation and stability.

**Communications (COM)**: Oversees data transmission to and from the satellite. 
<center>  
  <p>
    <img alt="birdsx-com" src="assets/images/birdsx-com.png" width="25%">
  </p>  
</center>

**Structure**: Designs and constructs the satellite’s physical frame.
<p>
  <img alt="birdsx-frame" src="assets/images/birdsx-frame.png" width="45%">
&nbsp;
  <img alt="birdsx-board-frame" src="assets/images/birdsx-board-frame-assembly.png" width="45%">
</p>

**Payload**: Manages mission-specific instruments or sensors.

**Backplane (BPB)**: Integrates all the subsystems and allows transfer of power and data to each of them.
<center>         
  <p>
    <img alt="birdsx-bpb" src="assets/images/bpb-birdsx.png" width="15%">
  </p>
</center>


## *Organizational Chart*
{: .no_toc }

```mermaid
flowchart TD
    A[Satellite] --> B(Ground Segment)
    A[Satellite] --> C(Space Segment)
    C --> D[Payload]
    C --> E[Main Bus]
    D --> |Member 8| G[Mission-1]
    D --> |Member 7| H[Mission-2]
    E --> |Member 1| I[Structure]
    E --> |Member 2| J[COM]
    E --> |Member 3| K[ADCS]
    E --> |Member 4| L[EPS]
    E --> |Member 5| M[OBC]
    E --> |Member 6| N[BPB]
```

## **4. What tools do we use in development?**
   - **Software**:
     - **Computer Aided Design (CAD) tools for Design**: Fusion 360
     - **Simulation Tools**: Thermal desktop, STK for mission analysis
     - **Programming Languages**: C/C++, Python 
     - **Programming Environment**: CCS Compiler, MPLAB IDE
     - **Communication Protocols**: UART, SPI
   - **Hardware**:
     - **Microcontrollers/Boards**: PIC MCUs, custom PCBs
     - **Power Systems**: Solar panels, battery packs
     - **Sensing Devices**: Magnetometers, gyroscopes for ADCS
   - **Version Control**: Git/ [GitHub] 

## [Getting Started]({{site.url}}/get-started){: .btn .btn-purple }

----

[GitHub Issues.]: https://github.com/BIRDSOpenSource/Build-A-Satellite/issues
[GitHub]: https://github.com/BIRDSOpenSource
[our Discussions channel on Github]: https://github.com/orgs/BIRDSOpenSource/discussions/categories/ideas
[BIRDS]: https://birds-project.com/
[get in touch with us.]: info@kyutech-laseine.net
