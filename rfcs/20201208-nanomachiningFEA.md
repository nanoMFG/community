
# nanoMFG Software Planning Document
<!-- Replace text below with long title of project:short-name -->
## Nano-Scale Metal Working FEA Tool: nanomachiningFEA
### Target Release: 05.12.21 : 05 27, 2021

## Development Team
<!-- Complete table for all team members 
 roles: lead, developer, reviewer
 status: active, inactive
-->
Name | Role | github user | nanohub user | email | status
---|---|---|---|---|---
Qinan Zhou | developer | xx | xx | qzhou24@illinois.edu | active
Elyas Goli | developer | xx | xx | goli@berkeley.edu | active
Elif Ertekin | developer | xx | xx | ertekin@illinois.edu | active
Hayden Taylor | developer | xx | xx | hkt@berkeley.edu | active
Placid Ferreira | developer | xx | xx | pferreir@illinois.edu | active

**nanoMFG Github Team(s):** 
**nanoHUB Group(s):**

## 1. Introduction
The nano-scale metal work FEA tool focuses on using finite element analysis to simulate machining and burnishing in nano-scale. 

### 1.1 Purpose and Vision Statement
<!-- Why are we building this tool?
What is the key benefit
How does it relate to existing tools and existing software?
How does it fit into the overall objectives for the nano **manufacturing** node?
Who will use this software?
-->
Metal working in nano-scale is hard to predict. The majority of finite element analysis work is concentrated on conventional metal working which has scales in millimeters. 
This tool relates to the existing tools and existing software by bringing the same underlying principle and modifying and applying them into nano-scale. 
This tool fits into the overall objectives for the nanoMFG node, because it addresses the question of predicting nano-machining and nano-burnishing behaviors. 
Researchers and industrial companies will use this software. 

### 1.2 References
<!--List any documents or background material that are relevant.  Links are useful. For instance, a link to a wiki or readme page in the project repository, or link to a uploaded file (doc, pdf, ppt, etc.).-->
https://en.wikipedia.org/wiki/Machining
https://en.wikipedia.org/wiki/Burnishing_(metal)

## 2 Overview and Major Planned Features
<!--Provide and overview characterising this proposed release.  Describe how users will interact with each proposed feature. Include a schematic/diagram to illustrate an overview of proposed software and achitecture componets for the project-->
The users will need to provide cutting parameters and tool gemeotries. Once received these, the software will run the simulation itself. The corresponding results will be provided to users. 

### 2.1 Product Background and Strategic Fit
<!--Provide context for the proposed product.  Is this a completely new projects, or next version of an existing project? This can include a description of any contextual research, or the status of any existing prototype application.  If this SPD describes a component, describe its relationship to larger system. Can include diagrams.-->
Finite element modeling and simulations for metal working, especially machining and burnishing, are widely and well studied. However, current study mainly focuses on conventional scale, i.e. milimeter scales, and high speeds. Thus, based on the previous study, this project is trying to modify the principles in the conventional scale and apply them into nanoscale. 

### 2.2 Scope and Limitations for Current Release
<!--List the all planned goals/features for this release.  These should be links to issues.  Add a new subsection for each release.  Equally important, document feature you explicity are not doing at this time-->
This software could only run in computer with Abaqus installed. Improvements will be made to overcome this limitation. 

##### 2.2.1 Planned Features

#### 2.2.2 Release Notes 
##### v#.#.#

### 2.3 Scope and Limitations for Subsequent Releases
<!--Short summary of  future envisioned roadmap for subsequent efforts.-->
To make this code open-source and free. (will be changed in the future)

### 2.3 Operating Environment
<!--Describe the target environment.  Identify components or application that are needed.  Describe technical infrastructure need to support the application.-->
Abaqus installed.  (will be changed in the future)

### 2.4 Design and Implementation Constraints
<!--This could include pre-existing code that needs to be incorporated ,a certain programming language or toolkit and software dependencies.  Describe the origin and rationale for each constraint.-->
Needs to access the cluster.  (will be changed in the future)

## 3 User Interaction and Design

### 3.1 Classes of Users
<!--Identify classes (types) of users that you anticipate will use the product.  Provide any relevant context about each class that may influence how the product is used: 
The tasks the class of users will perform
Access and privilege level
Features used
Experience level
Type of interaction
Provide links to any user surveys, questionnaires, interviews, feedback or other relevant information.-->
1. Researchers: Researchers need a way to better predict the behavior of metal under nano-machining and nano-burnishing. 
2. Industrial Companies: The metal working process used by industrial companies are highly customized. Thus, developing a new nanoscale model for each process is time-consuming and costly. Thus, industrial companies are looking for generic software to simulation the machining and burnishing process in nanoscale. 
Survey in Progress...

### 3.2 User Requirements
<!-- Provide a list of issue links to document the main set of user requirements to be satisfied by this release.  Use the user requirement template to draft thense issues.  A well written user requirement should be easy to justify (Rational) and should be testable.  List in order of priority as must have, should have or nice to have for each use case. -->
1. Abaqus 
2. Python 

### 3.3 Proposed User Interface
<!--Could include drawn mockups, screenshots of prototypes, comparison to existing software and other descriptions.-->
1. Abaqus 
2. Jupiter Notebook in the future

### 3.4 Documentation Plan
<!-- List planned documentation activities -->
Document the progress whenever this is a major improvement or change in the software. 

### 3.5 User Outreach Plan
<!-- List upcoming activities designed to elicit user feedback and/or engage new users.  Use issues for activities that will be completed this iteration-->
Contact us by e-mails. 

## 4. Data And Quality Attributes

### 4.1 Data Dictionary
<!--Summarize inputs and outputs for the application.-->
1. Input: Cutting parameters, tool geometries, materials
2. Output: stress distribution, forces, material recovery, workpiece profile

### 4.2 Usability and Performance
<!--Summarize usability requirements such as easy of adoption for new users (eg example data),  inline documentation, avoiding errors, efficient interaction, etc.  Describe performance expectations  and/or document challenges.  Note you can reference user requirements from above if needed. -->
Users have to get access to Abaqus in this stage, but this will become open source in the future. 
For the performance, at this stage, it requires cluster to do the calculation, and thus it is computationally intense. However, it will be improved in the future. 

### 4.3 Testing, Verification and Validation
<!--Describe What data is necessary to verify the basic functionality of the application.  Provide a testing plan that includes a list of issues for each planned activity.  Describe data sets that are needed to test validation.-->
Testing and verification of the model is based on real experimental data from some companies. 

### 4.4 Uncertainty Quantification
<!--Identify and document possible sources of uncertainty. Categorize with standard labels, such as parametric, structural, algorithmic, experimental, interpolation.
Develop a plan for measuring and documenting uncertainty, e.g., using forward propagation or inverse UQ, and showing it in the application, if applicable.-->
TBD. 
