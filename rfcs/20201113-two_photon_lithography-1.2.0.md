	# nanoMFG Software Planning Document
<!-- Replace text below with long title of project:short-name -->
## nanoMFG Tool for Two-Photon Lithography (TPL)
### Target Release: v1.2.0: Dec 31st, 2020

## Development Team
<!-- Complete table for all team members 
 roles: PI, developer, validation
 status: active, inactive
-->
Name | Role | github user | nanohub user | email | status
---|---|---|---|---|---
Kimani C. Toussaint, Jr. | PI | n/a | n/a | ktoussai@illinois.edu | active
Hemangg Singh Rajput | developer | singhra2 | n/a | singhra2@illinois.edu | active
Qing Ding | developer | Aerovane | n/a | qingding@illinois.edu | inactive
Varun Kelkar | developer | kvarun95 | n/a | vak2@illinois.edu | inactive
Mohammad Kabir | developer | mmkabir2 | n/a | mmkabir2@illinois.edu | inactive

## 1. Introduction
<!-- A simulation tool that captures the physics of TPL . -->

### 1.1 Purpose and Vision Statement
This is intended to be a software tool that captures the physics of TPL. The tool will be posted on the NanoHub. It also creates a database of photopolymers, which can be updated by end users. It enables the user to:
- Define experimental parameters
- Choose a suitable photopolymer from a drop-down menu
- Obtain optimized scan parameters for generating a 3D structure

### 1.2 References
1. J. Serbin, A. Egbert, A. Ostendorf, B. N. Chichkov, R. Houbertz, G. Domann, J. Schulz, C. Cronauer, L. Fröhlich, and M. Popall, "Femtosecond laser-induced two-photon polymerization of inorganic–organic hybrid materials for applications in photonics," Opt. Lett. 28, 301-303 (2003)
2. W. Martin McClain, "Two-photon molecular spectroscopy," Accounts of Chemical Research 7 (5), 129-135 (1974)
3. Zhou et al., "Mechanically stretchable and tunable metamaterial absorber," Applied Physics Letters, 9 (2015)

## 2. Overview and Major Planned Features

### 2.1 Product Background
This is an overview on the Nanoscribe TPL setup.

![Nanoscribe TPL Setup](https://github.com/nanoMFG/Two-photon-lithography/blob/planning_qingding/pic/Nanoscribe%20TPL%20Setup.jpg)





This is an overview of the mechanism behind TPL process.
![TPL Mechanism](https://github.com/nanoMFG/Two-photon-lithography/blob/planning_qingding/pic/TPL%20Mechanism.jpg)






There are two major steps in modeling the TPL tool. The first step (year 1) is completed in release v1.1.0. And the second step is decribed in Year 2 box.
![Modeling TPL](https://github.com/nanoMFG/Two-photon-lithography/blob/planning_qingding/pic/Modeling%20TPL.jpg)

#### 2.1.1 Release Notes v1.1.0
In v1.1.0 of the tool, a single voxel of the two-photon lithography process is simulated. To calculate a single voxel size, the function "calculate_voxel_params" is implemented to calculate the voxel length and diameter. This function is dependent on the pulse width, repetition rate, wavelength, exposure time, focal power of the input light source, and various material parameters like two photon polymerization cross section, refractive index of immersion fluid, etc.

This is a view of the voxel simulation result:
![Voxel Simulation](https://github.com/nanoMFG/Two-photon-lithography/blob/planning_qingding/pic/Voxel%20Simulation.jpg)


### 2.2 Scope and Limitations for Current Release 

#### 2.2.1 Planned Features of Release v1.2.0
In this release, the voxel simulation tool from v1.1.0 will be modified to include the uncertainty associated with several input parameters. For example, the laser power might be set at 30mW but there are some minor fluctuations in the laser power which might affect the voxel size. 
In this release, the wavelength, the laser power, the pulsewidth and the laser pulse repetition rate are assumed to be normally distributed around the mean and standard deviation values provided by the user. This information is then used to calculate the length and diameter of the voxel that is 1.96 standard deviation below and above the mean length and diameter. This allows the TPL tool to predict with a 95% certainty that the length and diameter of the voxel will fall in between a certain calculated range.      

#### 2.2.2 Release Notes v1.2.0
The function “uncertainty_quantification” is implemented to calculate the voxel length and diameter that is 1.96 standard deviation below and above the mean voxel length and diameter. The mean values are calculated by the “calculate_voxel_params” function that was implemented in the previous release. The function takes in all the inputs of the “calculate_voxel_params” along with the standard deviation values of the wavelength, laser power, pulsewidth and laser pulse repetition rate. 

Here is a view of the tool in its current form: 
![TPL tool v1.2.0] [INSERT PIC HERE]
### 2.3 Scope and Limitations for Subsequent Releases

For the current version, the normal distribution model is being used to quantify the uncertainty in the input parameters, but experiments would need to be carried out for developing a better model that can be used for uncertainty quantification. 
The next version of the tool will also move towards simulations of 2D and 3D structures using CAD models as input along with all the parameters required now.

### 2.4 Operating Environment 

The TPL tool uses Jupyter Notebook to run and users can access it directly from their browsers through the NanoHub website.

### 2.5 Design and Implementation Constrains

Due to the extra time required to generate plots for all the possible voxels, the development team has decided to show just 3 voxel plots that the user can scroll through. These are the mean value voxel, the voxel that is 1.96 standard deviation below the mean and the voxel that is 1.96 standard deviation above the mean.

## 3. User Interaction and Design  

### 3.1 Classes of Users

The primary users of this tool will be researchers who manufacture micrometer or sub-micrometer structures using two-photon lithography. They can use this tool to find out the size of their two-photon lithography voxel and make changes to their process parameters if necessary, without manufacturing their structures.
### 3.2 User Requirements

The requirement to use this tool is to have all the information about the input parameters that the tool needs. These are the wavelength of the laser, the laser power, the pulsewidth, the laser pulse repetition rate, the laser exposure time, the numerical aperture, the refractive index of the immersion fluid, the two-photon polymerization cross section, the radical density and the initiator density. 

### 3.3 Proposed User Interface

Here is a view of the proposed user interface:
![TPL tool v1.2.0 UI] [INSERT PIC HERE]

The user interface will have appropriate fields for entering all the input parameters, their mean and their standard deviation, if appropriate. It will also have a slider bar to scroll through the different voxel sizes that are simulated by the tool. Lastly, it will have two plots to show the distribution of the length and diameter of the voxel below the plot of the simulated voxel.

### 3.4 Documentation Plan

All code is written keeping best practices in mind. The codebase is well commented, the variables have descriptive names, proper indentation is used, and the code is broken down into several independent function blocks. 
Apart from the codebase itself, the development team has maintained this software planning document, and several PowerPoint presentations in the GitHub repository for documentation purposes. The software planning document will be updated regularly to reflect the current status of the tool.

### 3.5 User Outreach Plans

After the next version of the tool is published, we can ask researchers that use two-photon lithography technique to review the tool and provide some feedback that we can incorporate in the next version of the tool. Some of these research groups are at the University of Illinois at Urbana-Champaign, Brown University and Georgia Tech. 

## 4. Data and Quality Attributes 


  


