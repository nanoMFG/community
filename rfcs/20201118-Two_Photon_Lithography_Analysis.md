# nanoMFG Software Planning Document
<!-- Replace text below with long title of project:short-name -->
## The Coolest nanoHUB Tool: Two Photon Lithography Analysis
### Target Release: 12.15.2021 

## Project Team
<!-- Complete table for all team members 
 roles: lead, developer, reviewer
 status: active, inactive
-->
Name | Role | github user | nanohub user | email | status
---|---|---|---|---|---
Sixian Jia | developer | sixianj2 | sixianj2| sixianj2@illinois.edu | active
Yuhang Yang | developer| yang221 | yang221 | yang221@illinois.edu | active
Hemangg Singh Rajput | reviewer | singhra2 | n/a | singhra2@illinois.edu | active
Qing Ding | reviewer  | Aerovane | n/a | qingding@illinois.edu | inactive
Varun Kelkar | reviewer  | kvarun95 | n/a | vak2@illinois.edu | inactive
Mohammad Kabir | reviewer  | mmkabir2 | n/a | mmkabir2@illinois.edu | inactive




## 1. Introduction
Data Based Uncertainty Quatification and Process Capability Analysis for Two Photon Lithography

### 1.1 Purpose and Vision Statement
<!-- Why are we building this tool?
What is the key benefit
How does it relate to existing tools and existing software?
How does it fit into the overall objectives for the nano **manufacturing** node?
Who will use this software?
-->
To improve the utility and ultimate dissemination of our published TPL software tool, we have been developing a framework for which to incorporate (experimental) process variability in our simulation model in order to obtain insight on the repeatability of the TPL process. Our initial approach uses 3D geometric measurements of fabricated structures/features.The tool will provide:

1.Spatial distributions of geometric features.
(a)Height
(b)Radius
(c)Volume

2.Geometric deviation from the designed shape.

3.Summary of geimetric features and errors

### 1.2 References
<!--List any documents or background material that are relevant.  Links are useful. For instance, a link to a wiki or readme page in the project repository, or link to a uploaded file (doc, pdf, ppt, etc.).-->
 [1] Cumpston, Brian H., Sundaravel P. Ananthavel, Stephen Barlow, Daniel L. Dyer, Jeffrey E.
 Ehrlich, Lael L. Erskine, Ahmed A. Heikal et al. "Two-photon polymerization initiators for three-
 dimensional optical data storage and microfabrication." Nature 398, no. 6722 (1999): 51.
A47

 [2] Juodkazis, Saulius, Vygantas Mizeikis, Kock Khuen Seet, Masafumi Miwa, and Hiroaki Misawa.
 "Two-photon lithography of nanorods in SU-8 photoresist." Nanotechnology 16, no. 6 (2005): 846.
 
 [3] Tormen, Microelectron, L. Businaro, M. Altissimo, F. Romanato, S. Cabrini, F. Perennes, R.
 Proietti, Hong-Bo Sun, Satoshi Kawata, and E. Di Fabrizio. "3D patterning by means of
 nanoimprinting, X-ray and two-photon lithography." Microelectronic Engineering 73 (2004): 535-
 541.
 
 [4] Jhaveri, Shalin J., Jesse D. McMullen, Rint Sijbesma, Loon-Seng Tan, Warren Zipfel, and
 Christopher K. Ober. "Direct three-dimensional microfabrication of hydrogels via two-photon
 lithography in aqueous solution." Chemistry of materials 21, no. 10 (2009): 2003-2006.

[5] Montgomery, Douglas C. Statistical quality control. Vol. 7. New York: Wiley, 2009.
 
 [6] Chen, K. S., M. L. Huang, and R. K. Li. "Process capability analysis for an entire
 product." International Journal of Production Research 39, no. 17 (2001): 4077-4087.
 
 [7] Wu, CF Jeff, and Michael S. Hamada. Experiments: planning, analysis, and optimization. Vol. 552.
 
## 2 Overview and Major Planned Features
<!--Provide and overview characterising this proposed release.  Describe how users will interact with each proposed feature. Include a schematic/diagram to illustrate an overview of proposed software and achitecture componets for the project-->

### 2.1 Product Background and Strategic Fit
<!--Provide context for the proposed product.  Is this a completely new projects, or next version of an existing project? This can include a description of any contextual research, or the status of any existing prototype application.  If this SPD describes a component, describe its relationship to larger system. Can include diagrams.-->
TPL Mechanism

![Screen Shot 2020-11-10 at 1 24 10 AM](https://user-images.githubusercontent.com/71730024/98636077-1c792c80-22f4-11eb-89ce-608cf636f7ae.png)

Hardware Setup

![Screen Shot 2020-11-10 at 1 27 22 AM](https://user-images.githubusercontent.com/71730024/98635993-edfb5180-22f3-11eb-8c51-5b5ef39ac003.png)


### 2.2 Scope and Limitations for Current Release
<!--List the all planned goals/features for this release.  These should be links to issues.  Add a new subsection for each release.  Equally important, document feature you explicity are not doing at this time-->

In the current release, the tool is used to simulate the final shape of a CAD design geometry. For next version, the tool will use 3D geometric measurements to fabricate structures and features.

##### 2.2.1 Planned Features

1.Spatial distributions of geometric features
(a)Height
(b)Radius
(c)Volume

2.Geometric deviation from the designed shape

3.Summary of geimetric features and errors
### Current Progress
1.Spatial distributions of geometric features
![Screen Shot 2020-11-10 at 1 44 17 AM](https://user-images.githubusercontent.com/71730024/98637749-dd000f80-22f6-11eb-841b-a9ff00635cdf.png)

![Screen Shot 2020-11-10 at 1 44 24 AM](https://user-images.githubusercontent.com/71730024/98637753-dec9d300-22f6-11eb-869a-60c69e5ea4c1.png)

![Screen Shot 2020-11-10 at 1 44 30 AM](https://user-images.githubusercontent.com/71730024/98637758-e0939680-22f6-11eb-9a35-5833cc8a0ae6.png)

2.Geometric deviation from the designed shape

![Screen Shot 2020-11-10 at 1 45 03 AM](https://user-images.githubusercontent.com/71730024/98637761-e25d5a00-22f6-11eb-9078-1fe54cc099b7.png)

3.Summary of geimetric features and errors

![Screen Shot 2020-11-10 at 1 45 14 AM](https://user-images.githubusercontent.com/71730024/98637765-e38e8700-22f6-11eb-872a-c4c8ae830840.png)

### 2.3 Scope and Limitations for Subsequent Releases
<!--Short summary of  future envisioned roadmap for subsequent efforts.-->


### 2.3 Operating Environment
<!--Describe the target environment.  Identify components or application that are needed.  Describe technical infrastructure need to support the application.-->

The TPL Analysis tool uses Jupyter Notebook to run. Users can use the tool from Nanohub website or download the code from NanoMFG.


## 3 User Interaction and Design

### 3.1 Classes of Users
<!--Identify classes (types) of users that you anticipate will use the product.  Provide any relevant context about each class that may influence how the product is used: 
The tasks the class of users will perform
Access and privilege level
Features used
Experience level
Type of interaction
Provide links to any user surveys, questionnaires, interviews, feedback or other relevant information.-->

The researchers who use two photon lithography to generate micro/nanostructures will be the users of our tool. They could use our tool to generate the deometric deviation from the designed shape and get geimetric features and errors. Meanwhile, all uesful infomation will be summerize in a cvs file, users could download for futher analysis. 

### 3.2 User Requirements
<!-- Provide a list of issue links to document the main set of user requirements to be satisfied by this release.  Use the user requirement template to draft thense issues.  A well written user requirement should be easy to justify (Rational) and should be testable.  List in order of priority as must have, should have or nice to have for each use case. -->

The users who want to use the tool should design a sample which contain 5*5 hemispheres and all the hemispheres are identical. The useres need to use Keyence VK-X1000 3D laser scanning microscope to adopt for height measurement and save the height measurement in the format of a 768*1024 martix to upload the file in the tool. The users need to reocrd the deigned radius and input the designed radius in our tool. 

### 3.3 Proposed User Interface
<!--Could include drawn mockups, screenshots of prototypes, comparison to existing software and other descriptions.-->
Here is the example of geometric deviation from the designed shape.
The smooth surface is the designed hemisphere, the inner shape is the acutal shape generate from two photon lithography.

![Screen Shot 2020-11-10 at 1 45 03 AM](https://user-images.githubusercontent.com/71730024/98637761-e25d5a00-22f6-11eb-9078-1fe54cc099b7.png)

Our tool will cacluate the equivalent radius, the maximum height, and the acual volume of the hemisphere. 

### 3.4 Documentation Plan
<!-- List planned documentation activities -->


### 3.5 User Outreach Plan
<!-- List upcoming activities designed to elicit user feedback and/or engage new users.  Use issues for activities that will be completed this iteration-->

After the tool publihsed, we will ask the researchers who work on the two photon lithography to use our tool and give some feedback about the interface or the functions of the tool. Thus, we could improve some functions or the appearance of the tool for next version. 
## 4. Data And Quality Attributes

### 4.1 Data Dictionary
<!--Summarize inputs and outputs for the application.-->
1.Input: The csv file which is generated from VK-X1000 3D laser scanning microscope(height measurement)
2.Output: Spatial distribution of geometric feature in hight, radius, and volume. The geometric deviation from the designed shape and summary the geometric features and errors.
### 4.2 Usability and Performance
<!--Summarize usability requirements such as easy of adoption for new users (eg example data),  inline documentation, avoiding errors, efficient interaction, etc.  Describe performance expectations  and/or document challenges.  Note you can reference user requirements from above if needed. -->
Two Photon Lithography Analysis is a open source tool on nanoHub. It is easy to use for new users and avoiding calculation errors during the analysis progress. Besides, the tool use data visualization to help users more intuitive understand the errors between the degined model and the actual model. For performance expectation, the tool can summary the geometix features and errors but it can't know how to minimize the errors. This will be improved in the next version tool.

### 4.3 Testing, Verification and Validation
<!--Describe What data is necessary to verify the basic functionality of the application.  Provide a testing plan that includes a list of issues for each planned activity.  Describe data sets that are needed to test validation.-->
Ten test data files are provided on the tool. All the test datasets are raw data from the provious experiments.  User would use the testing data to verify the basic functionality of the tool. If the tool does not work, please double check the file format and the matrix dimension should be 768*1024 for height measurement.

### 4.4 Uncertainty Quantification
<!--Identify and document possible sources of uncertainty. Categorize with standard labels, such as parametric, structural, algorithmic, experimental, interpolation.Develop a plan for measuring and documenting uncertainty, e.g., using forward propagation or inverse UQ, and showing it in the application, if applicable.-->
