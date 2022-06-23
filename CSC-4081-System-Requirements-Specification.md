# System Requirements Specification

> This document contains a template structure for your system requirements specification. To use this outline, replace the description under each section heading with the information about your project, but keep all of the section headings to maintain the structure of the document. If a section does not apply to your project, keep the heading in your document, and just state that it is not applicable. (In some cases, we might discover later that your project does have requirements related to that section!) 

# Project Title 
*Author*

*Sponsoring Organization*

*@ mentions for those with read access to repo and want to be notified of updates*

## Introduction

### System Overview
Provides a brief overview of the system objectives and scope. Start by copying the first section from your project proposal (Purpose and Scope), and revise as necessary to reflect any changes and refinements since your proposal was submitted. 

### Human Resources
Provides a brief overview of the system objectives and scope. Start by copying the first section from your project proposal (Purpose and Scope), and revise as necessary to reflect any changes and refinements since your proposal was submitted. 

### Business Context 
If the project is being developed for an organization or business, describe the business or organization sponsoring the development of this product, including the business's mission statement and its organizational objectives or goals. 

## User Requirements (written for customers, may need user stories and/or use case diagrams)

### User Objectives
This section describes a list of objectives and requirements from the user's perspective. You may start by copying the second section from your project proposal (Functional Description), and revise it as necessary (e.g., must-include requirements for M.V.P. and should-include requirements). This may include a *wish list* (e.g, nice-to-haves) of desirable features, along with comments if there are questions about whether a feature is likely to be feasible or consistent with the overall organizational context. 

### Similar System Information
This section describes a list of objectives and requirements from the user's perspective. You may start by copying the second section from your project proposal (Functional Description), and revise it as necessary. This may include a "wish list" of desirable features, along with comments if there are questions about whether a feature is likely to be feasible or consistent with the overall organizational context. 

### User Characteristics
Describes the characteristics of the user community, including their expected expertise with computer systems and the application domain. 

## Functional or System Requirements
This section lists the functional requirements of your system or application. A functional requirement describes a desired behavior or effect of the system, in other words, what the system must do, but should not get into details about how it will be implemented. When starting your first draft, just list the requirements as you become aware of them in any order. As you revise this section and get feedback from your stakeholders and advisor, reorder the requirements so that they are listed **in ranked order**, listing the most critical requirements first, and for equally important requirements, list them in the order in which you think they should be completed when one depends on another. Each functional requirement should be specified in the following format: 

**A short imperative sentence stating something the system should do.**

-**Description (Function)**
A description of the desired capability, explaining it as unambiguously as possible.
-**Inputs**
A description of the desired capability, explaining it as unambiguously as possible.
-**Outputs**
Describe any data produced and its destination.
-**Criticality**
Describes how essential this requirement is to the overall system. 
-**Risks**
Describes the circumstances under which this requirement might not be able to be satisfied, and what actions can be taken to reduce the probability of this occurrence. 
-**Dependencies with this requirement**

**A short imperative sentence stating something the system should do.**

...

(Note: each functional or system requirement should be have an entry on the project board)

## Interface Requirements

(Tio: There are many methods to generate GUI mockups or diagrams that include SceneBuilder, Draw.io, Visio, etc., if needed to supplement any verbal descriptions)

### User Interfaces
Describes what types of human user interfaces are required (e.g., GUI, web interface, command line, or log data that should be produced for diagnostic purposes).

### Hardware Interfaces
Describes interfaces to specific hardware devices.

### Communications Interfaces
Describes network interfaces

### Software Interfaces
Describes any required software interfaces, such as a server, database, or specific APIs. You may want to use class diagrams here. Don't forget to include JavaDocs or Doxygen docs, man files, etc., in your project when you reach the implementation phase or implementation portion of the current sprint. 

## Non-functional Requirements (Other than those previously listed)
 
(Examples from Ian Sommerville's Software Enginnering book and/or augmented by your prof)

### Hardware Constraints
Describes any required software interfaces, such as a server, database, or specific APIs.

Size: Megabytes of memory, number and type of ROM chips, amount of storage, server specs, number of virtual machines, containers,  etc. 

### Performance Requirements
Specifies any time and memory constraints that must be satisfied for the system to be effective. 

Speed: Processed transactions/second, Processed transactions/second, Processed transactions/second, etc.

### System Environment Constraints
Describes any standards for which compliance is required, such as database, file formats, or network protocols that must be supported.

### Security Requirements
Describe what must be done to provide proper authentication into the software system and what must be done to provide proper authorization to functionality. Do not forget to include how the entire software system will be updated to prevent loss of confidenality, integrity, or availability in the production system.

### Reliability
Describe to what extent the system **will correctly provide** implmented services in probablistic terms (what service level does your sponsor need to the system to achieve). What mechanims will be needed to allow this level of reliability (auto-restart of services, load-balanacing/CDN, caching, test/deploy servers with rollback, etc.).   

Examples: mean-time-to-failure (MTTF), probability of unavailability, rate of failure occurrence, etc.

### Robustness
Time to restart after failure, percentage of events causing failure, or probability of data corruption on failure

### Availabilty
Describe the probability the system **will be up and running** and able to deliver the requested services to the user. 99% reliabilty only allows for three days and fifteen hours of downtime where as 99.9% reliabilty only allows eight hours and forty-five minutes of downtime in a year. It gets progressively more restrictive with additional *9s* or reliability.What mechanims will be needed to allow this level of availabilty (auto-restart of services, load-balanacing/CDN, caching, test/deploy servers with rollback, etc.)?   

### Safety
Describe how likely this system is likely to hurt, maim, or otherwise injure/kill the user. Even if the system isn't capable of physical injury, it might have the potential to cause emotional or psychological damage and those impacts should be described here. Do we need to submit this project for an internal board review given the impact of the system on human users?

### Maintenance
Describes any expectations for how the software should be written to facilitate the ongoing development of the system after its first version. This may include coding conventions, continuous integration systems, pre or post hook scripts, how files will be organized, etc. 

### Portability
Describes the range of operating systems and device types that should be supported.

### Extensibility
Describes any constraints on forward or backward compatibility with other systems.

### Development Process Constraints
Describes the software development environment to be used, including operating systems, programming languages, platforms, or libraries, indicating any reasons that these are required or preferred. What percentage of target dependent statements are likely to be in the system? Keep in mind there is often a difference between the system that you develop the software on and the target systems where the software will execute. 

## System Models
This section includes diagrams showing relationships between major system components and the environment. It may include one or more of the following: 

-Context Models: what is part of the system and what is not. Includes model diagrams and activity diagrams
-Interaction Models: user to inputs/outputs, software to other systems/environment or among components in a system. Includes use-case digrams and sequence diagrams)
-Structural Models: how the components of the system relate to one another in a static manner. Includes class diagrams (top-level, detailed, aggregation/generalization), component diagrams, deployment diagrams, package diagrams, profile diagrams, and composite structure diagrams.
-Behavorial Models: show the dynamic behavior of the system as it executes. It includes activity (for data-flow), state/state-machine diagrams (event-flow), or timing diagrams
-Entity-Retionship diagrams (for database design) with schema reduction and normalization to third-normal-form (3NF) or Boyd-Codd Normal Form (BCNF) dependening on need for preserving functional dependencies (FDs, essentially business/logic rules). 
