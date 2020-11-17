## nanoMFG RFC process

nanoMFG RFC submissions generally apply to pre-approved projects that have arrived via whitepaper or through nanoMFG node sponsorship.  The RFC process is used to facilitate community feedback as these projects progress and communicate broadly upcoming software releases and features.

1. Submit your current Software Planning Document (SPD) draft as a RFC via a GitHub pull request to community/rfcs directory.  The pull request should be from a branch that you create with some descriptive name into the master branch of the community repo. 

   Name your RFC file based on the [SPD template](https://github.com/nanoMFG/community/blob/master/rfcs/YYYYMMDD-descriptive-name.md) `YYYYMMDD-descriptive-name.md`, where
   YYYYMMDD is the date of submission, and ‘descriptive-name’ relates to the
   title of your RFC. For instance, if your software project is titled “nanocool”, and you are planning to release version 1.0.0, 
   you might use the filename `20200910-nanocool-1.0.0.md`. If you have images
   or other auxiliary files, create a directory of the form `YYYYMMDD-descriptive-name`
   in which to store those files. Note: if images are already included in a SPD draft and stored elsewhere in the nanoMFG organization, there is no need to duplicate them and re-link.

3. Apply a label: `phase n: Proposed` to indicate the current development phase of the project for which a RFC review is being requested. As a reminder:
*  Phase 1: Planning Review
* Phase 2: Design and Construction Review
* Phase 3: Code Review
•	Phase 4: Implementation Review

4. Notify the nanoMFG-dev slack channel and all projects stakeholders which could include project leads, target user communities, PIs and nanoMFG leadership.  Be sure to include GitHub handles for any additional desired reviewers in the project Team table with the role of “reviewer”.

5. A review committee will be formed, and permissions disseminated.  Once the RFC has been received, it will be opened by the review committee for a period of about 2 weeks.


After the initial phase 1 planning review, the PR will remain open.  The status will progress to the next phase and subsequent phase 2, 3 and 4 reviews opened as needed.  Only after the phse 4 implementation review will a SPD RFC be closed and merged as a final document in the `rfcs` directory.


