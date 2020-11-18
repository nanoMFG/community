# Phase 1 Planning Review Guide for nanoMFG Tools

## Overview

This document is intended for reviewers of nanoMFG Software Planning Documents (SPDs) that have completed documentation for the phase 1 planning of the project.

## Reviewer Roles and Review Objectives
### nanoMFG Maintainers:
the nanoMFG DevOps team will provide detailed reviews using the review criteria below as a guide.

### External collaborators, contributors or potential users:
 Reviewers that are not nanoMFG maintainers, but are also reviewing the SPD should offer most of their commentary on sections 3.1 and 3.2 (user classes, user requirements) as well as sections 2.2 and 2.3 and/or offer more general commentary on particular features that are of interest and whether the proposed software requirements and planned feature meet their needs and are complete and accurate.

 In some cases the offering new user/system requirement or features may also be warranted.

## Review Criteria
The following can be used as a template or rubric for a phase 1 review.  This template cna be copied and marked ed of as a review.  Specific line comment on the proposed SPD can also be offered.  Each review section should include explanation of any unchecked items.

### Github Accounts and Team(s)
- [ ] Project Team table includes all relevant stakeholders including project lead(s), developers and reviewers.
- [ ] Github handles are provided for all team members
- [ ] Roles are provided for all team members listed
- [ ] Contact info is provided for each team member (in order of importance):
  - [ ] github handle
  - [ ] nanoHUB username
  - [ ] slack handle
  - [ ] email

### Project Goals and Mission Statement
This section should provide a concise and clear answer to the following questions:
- [ ] Why are we building this tool?
- [ ] What is the key benefit
- [ ] How does this project relate to existing tools and existing software?
- [ ] How does this project benefit the nano **manufacturing** community at large?
- [ ] Who will use this software?

### License
- [ ] A standard license file has been added named "LICENSE".  The recommended licenses are: MIT or apache2
- [ ] Copyrights notices reflect the appropriate parent institution for example: `Copyright 20xx University of Illinois`, or `Copyright 20xx The Regents of the University of California`

#### References
https://copyright.illinois.edu/  
https://copyright.universityofcalifornia.edu/  

### User Classes: Section 3.1
Descriptions of user classes are critical for designing quality features that address the intended user(s) requirements.  Care should be taken during phase 1 to carefully consider the intended set of users of the project.  Below are a set of criteria to use when evaluating each user class:  

- [ ] The tasks the class of users will perform are considered.
- [ ] Access and privilege level (if relevant).
- [ ] Features used and frequency on interaction.
- [ ] Experience/knowledge level.
- [ ] Type of interaction (education, research, other…) and platform (nanoHUB, API, local use, etc.)

### User/System Requirements
There is no exact formula for an excellent user requirement, this guide is intended to help reviewer provide constructive feedback on how well the requirements communicate what the author intended as well as how clear, accurate, unambiguous and complete the requirements are. 

- [ ] Each user requirement is complete and unambiguous.
  - [ ] All information needs to understand the requirement and whom it affects.
  - [ ] System or user perspectives are okay but again should by unambiguous with clear phrasing such as "the system shall" or "user x shall".
- [ ] Requirements are correct: They accurately reflect a capability that will meet some stakeholder(s) needs.
- [ ] A clear value that the proposed capability provides to stakeholders the is communicated.
- [ ] User requirements make clear connections to user classes defined in section 3.1.

### User Outreach
This is an often overlooked aspect of the planning process and reviewers should expect to offer some guidance on this section.  In addition the nanoMFG node reviewers should include outreach activities that are supported by the node such as the nanoHUB newsletter and outreach to the nanoMFG community.
- [ ] The outreach plan is specific mentioning user classes or specific labs or courses.
- [ ] Does the plan have a timeline?
- [ ] Does the plan mention specific team members that will perform the outreach activities
- [ ] Does the plan describe how these outreach efforts will be used to improve the project outcomes.