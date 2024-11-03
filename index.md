---
title: Getting Started
layout: home
---

# *Getting Started Overview*
{: .no_toc }

## *So, you want to build a satellite?*
{: .no_toc }

{: .caution }
We are trying to make this resource as comprehensive as possible but this is by no means the only resource you should refer to when starting your work.


- Table of Contents
{:toc}


## Introduction
{: .no_toc }
### We are creating an environment for sharing knowledge and ideas.
{: .no_toc }
By using the Open Source Satellite platform as the means to advance the next phase of low-cost, high-capability satellite missions, we hope to pique interest and increase access to information that will inspire the next generation of mission creators and end users.

To help you create your own open source satellite mission, we are building a library of resources that will cover the entire mission lifetime from start to finish. 

If you would want to contribute to, or work with the birds-project.com community in order to assist in developing this solution, please get in touch with us.


## **1. Project Overview**
   - **Project Name**: [Name of the satellite project]
   - **Objective**: [Brief description of the project's primary goal, e.g., "Developing a CubeSat for Earth observation to support agricultural data collection."]
   - **Mission Scope**: [Explain the mission, e.g., "Launch and operate a 3U CubeSat equipped with sensors for remote sensing applications."]
   - **Project Status**: [Current status, such as "In design phase," "Prototyping," or "Pre-launch."]
   - **Key Stakeholders**: [List the main institutions, agencies, or partners involved.]

## **2. Team Structure**
   - **Subsystem Teams**:
     - **OBC (On-Board Computer)**: Handles the satellite’s core computing needs.
     - **EPS (Electrical Power System)**: Manages power generation, storage, and distribution.
     - **ADCS (Attitude Determination and Control System)**: Controls satellite orientation and stability.
     - **COM (Communications)**: Oversees data transmission to and from the satellite.
     - **Structure**: Designs and constructs the satellite’s physical frame.
     - **Payload**: Manages mission-specific instruments or sensors.
   - **Team Leads and Contacts**:
     - [Name and contact for each subsystem lead]
   - **Organizational Chart**: [Insert a diagram or link to a visual chart of team roles.]

```mermaid
graph TD;
    accTitle: the diamond pattern
    accDescr: a graph with four nodes: A points to B and C, while B and C both point to D
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```


++++
<pre class="language-mermaid">
graph TD;
    accTitle: the diamond pattern
    accDescr: a graph with four nodes: A points to B and C, while B and C both point to D
    A-->B;
    A-->C;
    B-->D;
    C-->D;
</pre>
++++

## **3. Key Technologies and Tools**
   - **Software**:
     - **CAD for Design**: [e.g., SolidWorks, AutoCAD]
     - **Simulation Tools**: [e.g., ANSYS, STK for mission analysis]
     - **Programming Languages**: [e.g., C/C++, Python for software development]
     - **Communication Protocols**: [e.g., CCSDS, CAN bus]
   - **Hardware**:
     - **Microcontrollers/Boards**: [e.g., CubeSat kit, custom PCBs]
     - **Power Systems**: [e.g., Solar panels, battery packs]
     - **Sensing Devices**: [e.g., Magnetometers, gyroscopes for ADCS]
   - **Version Control**: [e.g., Git/GitHub repository link]

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

---

**End of Guide**

---

This template ensures that new members have a clear pathway for getting acquainted with the project, accessing essential resources, and understanding their roles and expectations.

----

[GitHub]: https://docs.github.com/en/pages
[README]: https://github.com/BIRDSOpenSource/Build-A-Satellite/blob/main/README.md
