---
title: Getting Started
layout: home
---

# *Getting Started*
{: .no_toc }

{: .caution }
We are trying to make this resource as comprehensive as possible but this is by no means the only resource you should refer to when starting your work.

- Table of Contents
{:toc}

## **1. Introduction**
   The BIRDS program, developed in the Laboratory of Lean Satellite Enterprises and In-Orbit Experiment at Kyushu Institute of Technology (Kyutech), embodies a global initiative focused on advancing space development and educational opportunities for emerging spacefaring nations. To ensure mission success, rigorous testing and validation processes are vital for each subsystem of the satellite. 

   This guide is intended to facilitate a comprehensive understanding of the usage of BIRDS Bus subsystem testing documents, empowering team members and collaborators to follow standardized procedures for reliable subsystem performance.

   This document outlines the purpose, structure, and practical steps for using the testing process and procedural guides for subsystems such as the On-Board Computer (OBC), Electrical Power System (EPS), Attitude Determination and Control System (ADCS), Communications (COM), and the structural components of BIRDS satellites.

### We are creating an environment for sharing knowledge and ideas.
{: .no_toc }
By using the Open Source Satellite platform as the means to advance the next phase of low-cost, high-capability satellite missions, we hope to pique interest and increase access to information that will inspire the next generation of mission creators and end users.

To help you create your own open source satellite mission, we are building a library of resources that will cover the entire mission lifetime from start to finish. 

If you would want to contribute to, or work with the birds-project.com community in order to assist in developing this solution, please contibute to the [our Discussions channel on Github] or [get in touch with us.]

## **2. What are the phases of a satellite?**
  The development and deployment of a satellite involve a series of carefully structured phases to ensure the mission's success. From initial concept discussions to final pre-launch verifications, these phases guide teams through designing, building, and testing the satellite to meet stringent space industry standards. 
    
  Each phase acts as a checkpoint to confirm that requirements are met and potential risks are mitigated. Understanding the phases — including the Mission Definition Review (MDR), Preliminary Design Review (PDR), Critical Design Review (CDR), and Flight Model Testing (FMT) — is essential for satellite teams to manage the complexity of satellite engineering and increase the likelihood of achieving mission goals.

[![](https://mermaid.ink/img/pako:eNqNVU2PmzAQ_SuWDz3BCkPIB7dts6kqFbXaVQ-tuFh4QqyCTW2TNo32v3eApOySsLu5xGZmnt97M5gjzbUAmlDf9zOVa7WVRZIpQtwOKkiIAp2pLlZw5VwbwZh0JZAH7qAspQOSyhKs0wpsHxcY2WhTcUfId_z5aeqv133MQu6kxmUqrW0XeGYOtSMC9lDqGkSfl67v2z-SVGdwj-RGOo_w0CNhwGZ-wPww8MjsVHFLHLc_sYKzIYHFHlmJ50cPxHu9jeHdcwFWFqrP5UqjA-YE2fIYEAlp8UegZzk1P5SaixMY4oizsgqU6_YO9UhV9PVfTzqvCY3OOkI_GnSOqSWDGS2ziI2YvW_sUwoT-tC2rcMHnbuLEcSdKqQCMMiaVDgvJZHKQXHy7d1zRR8mO3cW87RrV4ic01jY6mHhZPus3rrf3MClvE36IoXID1ZvohBEnaXLEYVNKYude92KF5DDeScuHiF_NLrBEbEH66AaBBrYy3a8XmsejkkUXDRP-E77d6fJm4QYvMH3h0UjlC819Bp5SeqSt1IN7IAby8s3QM6uNHJj4FcDKj_ge6iNkKr38NPt_bdpxGFK42hyMLAtcg_mQJwmn3mj8h2pjd5LAeZ1rmzuXVDtQaZrWTBl1ws140PW0ta6s5N6tAK8P6XAm_nYZmW0u5AzmuBSwJY3pctoph4xlTdOPxxUThNnGvAojlCxo8mWlxZ3Td1ex2vJcUar_09BSKdN2t_93SfAozVXNDnSPzRhLL5ZzIJluFzF82AWLpYePdAEtzcsXsyiKF7NozAOHz36V2tEZV31j27dknj8B6oH7-0?type=png)](https://mermaid.live/edit#pako:eNqNVU2PmzAQ_SuWDz3BCkPIB7dts6kqFbXaVQ-tuFh4QqyCTW2TNo32v3eApOySsLu5xGZmnt97M5gjzbUAmlDf9zOVa7WVRZIpQtwOKkiIAp2pLlZw5VwbwZh0JZAH7qAspQOSyhKs0wpsHxcY2WhTcUfId_z5aeqv133MQu6kxmUqrW0XeGYOtSMC9lDqGkSfl67v2z-SVGdwj-RGOo_w0CNhwGZ-wPww8MjsVHFLHLc_sYKzIYHFHlmJ50cPxHu9jeHdcwFWFqrP5UqjA-YE2fIYEAlp8UegZzk1P5SaixMY4oizsgqU6_YO9UhV9PVfTzqvCY3OOkI_GnSOqSWDGS2ziI2YvW_sUwoT-tC2rcMHnbuLEcSdKqQCMMiaVDgvJZHKQXHy7d1zRR8mO3cW87RrV4ic01jY6mHhZPus3rrf3MClvE36IoXID1ZvohBEnaXLEYVNKYude92KF5DDeScuHiF_NLrBEbEH66AaBBrYy3a8XmsejkkUXDRP-E77d6fJm4QYvMH3h0UjlC819Bp5SeqSt1IN7IAby8s3QM6uNHJj4FcDKj_ge6iNkKr38NPt_bdpxGFK42hyMLAtcg_mQJwmn3mj8h2pjd5LAeZ1rmzuXVDtQaZrWTBl1ws140PW0ta6s5N6tAK8P6XAm_nYZmW0u5AzmuBSwJY3pctoph4xlTdOPxxUThNnGvAojlCxo8mWlxZ3Td1ex2vJcUar_09BSKdN2t_93SfAozVXNDnSPzRhLL5ZzIJluFzF82AWLpYePdAEtzcsXsyiKF7NozAOHz36V2tEZV31j27dknj8B6oH7-0)


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

### *Flight Model Testing (FM)*
- Flight Model Testing is the phase where the actual satellite, known as the Flight Model (FM), undergoes a series of rigorous tests to validate its performance under conditions that simulate the space environment. This is the final verification before launch.
- **Key Activities**:
  - **Functional Testing**: Verifying that each subsystem and the satellite as a whole function as expected.
  - **Environmental Testing**:
    - **Thermal Vacuum (TVAC) Testing**: Ensuring the satellite can withstand the extreme temperatures and vacuum conditions of space.
    - **Vibration Testing**: Testing for structural integrity under launch conditions to ensure it can survive the launch vibrations.
    - **Electromagnetic Compatibility (EMC) Testing**: Ensuring the satellite's electronic systems do not interfere with one another and comply with communication standards.
  - **Deployment Testing**: Verifying the proper deployment of antennas, solar panels, or other movable parts.
- **Outcome**: Confirmation that the satellite is ready for launch. Any failures during this phase may require redesign, rework, or additional testing until issues are resolved and the satellite meets all operational standards.

### *Conclusion*
{: .no_toc }
These phases create a structured pathway from conceptualization to launch, with each review and testing stage serving as a critical checkpoint. The **Mission Definition Review** sets the scope, the **Preliminary Design Review** checks the initial design feasibility, the **Critical Design Review** finalizes the detailed design, and **Flight Model Testing** ensures that the satellite is robust and mission-ready. This structured approach helps in mitigating risks, ensuring quality, and promoting mission success.

## **3. What is in the BIRDS bus?**
- The bus includes the following key components:
     - **On-Board Computer (OBC)**: Handles the satellite’s core computing needs.
     - **Electrical Power System (EPS)**: Manages power generation, storage, and distribution.
     - **Attitude Determination and Control System (ADCS)**: Controls satellite orientation and stability.
     - **Communications (COM)**: Oversees data transmission to and from the satellite.
     - **Structure**: Designs and constructs the satellite’s physical frame.
     - **Payload**: Manages mission-specific instruments or sensors.
     - **Backplane (BPB)**: Integrates all the subsystems and allows transfer of power and data to each of them.

## *Organizational Chart*
{: .no_toc }
[![](https://mermaid.ink/img/pako:eNp1kTtrwzAURv_KRVMK8ZD0BR4K8YP05cbgbrIH1bq2BbYUZIkSovz3qmkIbXE0Sd85izh7UiuOJCRNrz7rjmkD70kpwZ8VLZjBvhcGKwiCB4hma62s5FBgO6A0Vxe8eFZsWY3_tPjIEpqzXa8Yr36vKc2YkBDZ8TQnx9llOHyghjsHa5qJcRRKBotJ5d7B41lZnpT0j7Jw8EQLo21trMZJZengmcabbBJeO3ihqyQuJumNg1ea5tPw1kFGN1F8Cb7RKI8qMicD6oEJ7nvsv9WSmA4HLEnorxwbZntTklIevMqsUcVO1iT0X8I58WnajoQN60f_slvuoySCtZoN5xW5MEpnP8WP4Q9f4pycZg?type=png)](https://mermaid.live/edit#pako:eNp1kTtrwzAURv_KRVMK8ZD0BR4K8YP05cbgbrIH1bq2BbYUZIkSovz3qmkIbXE0Sd85izh7UiuOJCRNrz7rjmkD70kpwZ8VLZjBvhcGKwiCB4hma62s5FBgO6A0Vxe8eFZsWY3_tPjIEpqzXa8Yr36vKc2YkBDZ8TQnx9llOHyghjsHa5qJcRRKBotJ5d7B41lZnpT0j7Jw8EQLo21trMZJZengmcabbBJeO3ihqyQuJumNg1ea5tPw1kFGN1F8Cb7RKI8qMicD6oEJ7nvsv9WSmA4HLEnorxwbZntTklIevMqsUcVO1iT0X8I58WnajoQN60f_slvuoySCtZoN5xW5MEpnP8WP4Q9f4pycZg)


## **3. What tools do we use in development?**
   - **Software**:
     - **Computer Aided Design (CAD) tools for Design**: Fusion 360
     - **Simulation Tools**: Thermal desktop, STK for mission analysis
     - **Programming Languages**: C/C++, Python 
     - **Communication Protocols**: UART, SPI
   - **Hardware**:
     - **Microcontrollers/Boards**: PIC MCUs, custom PCBs
     - **Power Systems**: Solar panels, battery packs
     - **Sensing Devices**: Magnetometers, gyroscopes for ADCS
   - **Version Control**: Git/ [GitHub] 

## **4. Getting Started Steps**
1. **Read the Documentation**:
   - Visit the [project’s documentation site link] for detailed guides and subsystem overviews.
2. **Access the Project Repository**:
   - **Link**: [Insert GitHub/GitLab link]
   - **How to clone**: `git clone [repository link]`
3. **Set Up Development Environment**:
   - **For Software**:
     - Install [list necessary IDEs or software, e.g., Visual Studio Code, Keil uVision].
     - Clone and navigate to relevant project directories.
   - **For Hardware**:
     - [Details on accessing lab facilities or prototyping stations]
4. **Join Communication Channels**:
   - **Main Channel**: [e.g., Slack, Discord link]
   - **Subsystem Groups**: [e.g., EPS team Slack channel]
5. **Schedule Introductory Meetings**:
   - Contact [name/role] for orientation calls or training sessions.

## **5. Project Workflow and Guidelines**
   - **Development Process**: [e.g., Agile workflow description, sprint planning]
   - **Task Assignments**: Use [tool, e.g., Jira, Trello] for tracking tasks.
   - **Code Contribution Guidelines**:
     - Ensure code meets project standards outlined in [link to contribution guide].
     - Submit pull requests to [branch, e.g., `develop` branch] for review.
   - **Testing Procedures**:
     - Each subsystem has its test protocols found [link to test documentation].
   - **Documentation**:
     - Follow templates provided in the [link to documentation folder].

## **6. Standards and Compliance**
   - **Industry Standards**:
     - Ensure compliance with [e.g., CubeSat Design Specification, NASA standards].
   - **Safety and Quality Assurance**:
     - Follow the quality assurance plan in [link to QA guide].
   - **Regulatory Guidelines**:
     - Be aware of launch provider requirements and national/international space regulations.

## **7. Resources and Further Reading**
   - **Internal Wiki**: [Link to project wiki]
   - **Training Material**: [Link to onboarding videos or slides]
   - **Reference Papers**: [Include links or references to related technical papers]
   - **Technical Support**:
     - For assistance, contact [technical lead’s name and email].

## **8. FAQs**
   - **How do I join the project?**
     - Contact [relevant email/contact link].
   - **Where can I find the project timeline?**
     - View the project roadmap [link to Gantt chart or schedule].
   - **How do I report issues or bugs?**
     - Use [e.g., GitHub Issues or dedicated bug-tracking tool].

## **9. Contacts and Support**
   - **Project Manager**: [Name, email]
   - **Subsystem Leads**: [Name, role, contact information]
   - **General Inquiries**: [General support email or contact form link]



----

[GitHub]: https://github.com/BIRDSOpenSource
[our Discussions channel on Github]: https://github.com/orgs/BIRDSOpenSource/discussions/categories/ideas
[get in touch with us.]: info@kyutech-laseine.net