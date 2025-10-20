# RCP Internship Program - Intake 13 - Semester 2 2025 (In Progress)

This is the list of projects for this intake. Here you will see:
- Summary of the problem and the work done in the project
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation.
- Links to the project management tool with the tasks shown

These reports are written by the group to help share information to future interns and interested parties.

For more examples, see the [Intake 11 - Summary Report Page](https://wehi-researchcomputing.github.io/intakes/11-Summer-2024-2025/)

Please [update and do a pull request for this page via Github here](https://github.com/WEHI-ResearchComputing/WEHI-ResearchComputing.github.io/blob/main/intakes/13-Semester-2-2025/index.md).

# AIVE

### OBJECTIVE
Our team was divided into two groups, each tasked with their own objectives. 

#### Organelle Segmentation
The objective for this group was to contribute to the AIVE project by addressing the intensive manual effort required for organelle segmentation in microscopy images. Identifying the structures of organelles within electron microscopy (EM) images is an important task in the AIVE pipeline which is largely done through manual segmentation- which is time consuming - rather than Machine Learning techniques such as Deep Learning Models due to insufficient investment in the matter. The task included exploring and evaluating the various software tools that can be used to perform segmentation of 3D EM images, thus allowing researchers to determine its viability in the AIVE workflow’s integration requirements. We created documentation regarding the usage of such tools, the results obtained, and observations such as their performance ability and technical capabilities.  

#### AI Probabilities and AIVE Integration
The second group’s objective was to streamline the AIVE workflow in WEKA. The motivation comes from knowing that in the current workflow, AIVE is a separate step from AI predictions to enhance the results. The goal was to explore WEKA to determine whether adding an extra layer to the model can integrate the AI predictions with the original EM image.  
For AIVE integration, one main task was to get the AI segmentation done in WEKA which includes training and evaluating a Random Forest classifier and getting the probability maps per class. The second main task was to preprocess the raw EM image using Fiji/ImageJ which includes applying contrast normalisation and denoising techniques.


### WHAT WE DID AS A GROUP
#### Comprehending the AIVE Workflow
As a group, we first reviewed the project background, research paper, and previous interns' work to get a clear understanding of our starting point. After this we began narrowing down the problem space to decide what we would work on, eventually landing on the two objectives mentioned. 

#### Tasks Undertaken:
-	Investigating various segmentation tools: We focused primarily on Empanada and microSam and began by testing the ML models provided by these software tools in their capability to segment FIB-SEM images. 
-	Develop Scripts for file conversion: Python scripts were written for conversions in relation to .tif format files. Specifically, Zarr to tiff and tiff to NumPy arrays.
-	Developed a model runner: A model runner that allows users to run multiple empanada models at the same time was implemented for convenience.
-	Setting up and testing workflows for 3D image data: Setup a  minimal reproducible pipeline: load → encode→ run models → merge → export
-	Documenting technical setups, challenges, and recommendations: All details related to the process, results achieved, and any notable observations as well as insights were recorded in documentation to be referred to. 
-	Sharing progress and insights in regular group meetings: We had regular group meetings amongst the team members to discuss our progress and to decide the next steps. We conveyed any issues and discoveries that we made during our experience and learned how to employ effective teamwork and communication to achieve results. 

We collaborated actively to identify bottlenecks, benchmark results, and keep documentation up to date for both future interns and project integration.

### FINAL STATUS
#### Organelle Segmentation
By the end of the internship, we had tested and documented the initial analysis of tools for organelle segmentation. We established a reproducible workflow, highlighted tool limitations, and proposed recommendations for further improvements.
While initial tool analysis objectives were achieved, additional development will be needed for full automation and deeper integration with the wider AIVE project
#### AI Probabilities and AIVE Integration
By the end of the internship, we were able to partially reproduce the AIVE core workflow that covers 3 main complex steps including AI segmentation, data preprocessing and voxel multiplication. Unlike AIVE original workflow, we were able to integrate AI segmentation and the voxel multiplication within WEKA by using a mathematical expression tool. 


## Key links
- [Final presentation video](https://wehieduau-my.sharepoint.com/personal/mosbergen_r_wehi_edu_au/_layouts/15/stream.aspx?id=%2Fpersonal%2Fmosbergen%5Fr%5Fwehi%5Fedu%5Fau%2FDocuments%2FRecordings%2FAIVE%20Weekly%20Project%20Meeting%2D20251007%5F150733%2DMeeting%20Recording%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E81ec71a7%2De37d%2D4d53%2Da7ad%2Db07b1cd30418&ga=1)
- [Final presentation slides](https://wehieduau.sharepoint.com/:b:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/AIVE/2025%20Semester%202/AIVE%20-%20Sem%202%202025%20Final%20presentation.pdf?csf=1&web=1&e=gNjPGx)
- [Link to individual learning plans](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/AIVE/2025%20Semester%202/ILPs?csf=1&web=1&e=qrYrGb)
- [Link to technical diaries](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/AIVE/2025%20Semester%202/Technical%20Diary?csf=1&web=1&e=bNCcZH)
- [Link to Github repos](https://github.com/MitochondRuna/AIVE-Intro/tree/WEHI-Internship-S2-2025)
- [Semester 2 2025 Folder](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/AIVE/2025%20Semester%202?csf=1&web=1&e=Iq6CnZ)

# BioNix

OBJECTIVE
The research project worked to boost bioinformatics workflow reproducibility through its development of BioNix which operates as a Nix package manager extension.  BioNix enables scientists to create reproducible environments for complex scientific analyses which can be shared and version controlled. Our main goal was to find the barriers of computational reproducibility and make useful improvements by adding documentation to code and implementing testing and packaging.

WHAT WE DID AS A GROUP
As a team, we explored the Nix ecosystem, including Bash scripting, Nix, Nixpkgs, and BioNix. The learning process started with a challenging slope because we lacked experience with these tools. We concentrated on: 
•	Understanding how Nix ensures consistent builds and dependency management.
•	Exploring reproducibility challenges in existing bioinformatics workflows.
•	Testing and documenting small, reproducible pipelines to demonstrate workflow consistency.
•	Improving onboarding materials by creating an “Introduction to BioNix Project” page, which provides guidance on installation, key concepts, and troubleshooting.
•	Maintaining detailed technical diaries to record progress, errors, and solutions for future contributors.
We worked collaboratively, shared progress in regular meetings, and updated documentation to support long-term project continuity and accessibility. 

HOW FAR WE GOT
By the end of the project, we achieved several tangible outcomes:
•	Developed a foundational understanding of reproducible build systems and workflow management using Nix and BioNix.
•	Demonstrated understanding of genome alignment conecepts and workflow.
•	Investigated reproducibility barriers in packaging complex bioinformatics tools, such as Gridss
•	Created and published onboarding documentation on GitHub to support new users and interns with minimal programming background.
Although full integration of advanced tools like Gridss into BioNix remains ongoing work, the team established a reproducible foundation, identified technical bottlenecks, and provided documentation that will streamline future development.
 
FINAL INSIGHTS
Through this project, we learned how to apply reproducibility principles in real-world bioinformatics contexts.
We moved beyond traditional learning styles to self-directed exploration, iterative testing, and reflective documentation.
Our collective effort resulted in practical contributions to BioNix’s infrastructure and onboarding resources, setting the stage for continued development by future contributors.

## Key links
- Final presentation video 
- [FInal presentation slides](https://wehieduau.sharepoint.com/:p:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc.aspx?sourcedoc=%7B9732F922-1FA2-4B54-9DF1-2573C7E76867%7D&file=BioNix%20Final%20Presentation%20Sem2%202025.pptx&action=edit&mobileredirect=true)
- [Link to individual learning plans](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FBioNix%20Introduction%2FBioNix%202025%20sem%202&viewid=afd55542%2D8e3a%2D4327%2D95f9%2D63450ae10d2a&web=1&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069)
- [Link to technical diaries](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FBioNix%20Introduction%2FBioNix%202025%20sem%202&viewid=afd55542%2D8e3a%2D4327%2D95f9%2D63450ae10d2a&web=1&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069)
- Link to Github repos - https://github.com/WEHI-ResearchComputing/BioNix-GettingStarted/wiki , https://github.com/ShreyasYadav-stats/Introduction-to-BioNix---getting-started 

# Duplex Sequencing

Our objective was to embed duplex-specific QC metric generation and reporting into the core pipeline in a reproducible and version-controlled way, improving upon earlier approaches that operated outside the main workflow. Duplex-specific metrics are currently calculated outside the main processing pipeline using custom R markdown, which are neither containerized nor version-controlled, making them difficult to reproduce and maintain. Additionally, some of these scripts rely on GPL-licensed components, which conflict with the MIT license of the in-house duplex pipeline, creating licensing incompatibilities. The Duplex QC results were also only available in standalone R-generated reports, while standard read-level metrics were presented in MultiQC. This fragmentation can make it harder for users to assess experimental quality efficiently.
 
To resolve these issues, we modularized the R Markdown notebook into a standalone R script to improve computational efficiency, enhance version control, facilitate automation within pipelines, and simplify testing. This was packaged within a Docker container to ensure reproducibility and compatibility by removing GPL-licensed dependencies. A custom MultiQC plugin was developed to render duplex-specific metrics and plots directly within the Duplex MultiQC report generated after consensus sequence creation, while leaving the standard read-level QC report unchanged. This integration ensures that visuals are clear, accessible, and tailored specifically for duplex quality assessment.
 
How far we got was completing all the planned work, including refactoring the R scripts, containerizing the workflow, developing the custom MultiQC plugin, and integrating everything into the main pipeline. The system has been tested, with team members reproducing each other’s results to ensure consistency and reliability. However, there remains considerable potential for extension on all fronts — from expanding the testing framework, to customizing the MultiQC plugin with additional metrics and visuals, as well as further optimizing the pipeline integration.

## Key links
- [Final presentation video](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/EeV_BzCx_0FBnzkZm_NuuXMBHp7nvgy9Ixh3mlaUMjAZSg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=f0t3BS)
- [Final presentation slides](https://www.canva.com/design/DAG0c0yTlyA/B2FPIQQAbQznB3_4JKls7g/edit?utm_content=DAG0c0yTlyA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- [Link to individual learning plans](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Duplex%20Sequencing/ILP%20Semester%202,%202025?csf=1&web=1&e=xoUv7y)
- [Link to technical diaries](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Duplex%20Sequencing/Technical%20Diaries%20Semester%202,%202025?csf=1&web=1&e=d9noTY)
- Link to Github repos: [duplex-seq-pipeline (Repo A)](https://github.com/WEHIGenomicsRnD/duplex-seq-pipeline), [G000204_duplex (Repo B)](https://github.com/WEHIGenomicsRnD/G000204_duplex), [calculate-duplex-metrics (Repo C)](https://github.com/Jahnavi1122/calculate-duplex-metrics/tree/dylan/calc-duplex-metrics-NanoMB1Rep1), [MultiQC plugin (Repo D)](https://github.com/Jahnavi1122/MultiQC_Plugin/tree/Sem2_2025)
- [Additional R_CLI and Plugin Docs](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Duplex%20Sequencing/Additional%20Documentation%20-%20Plugin%20and%20RCLI%20(Sem2_2025)?csf=1&web=1&e=s2oLRc)
- [Project FAQ](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Duplex%20Sequencing/Project_FAQ.docx?d=wd985b45c6fb24bff9f8cc275e5519c9c&csf=1&web=1&e=3snPEN)
- [Meeting Docs](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Duplex%20Sequencing/Sem2_2025_Meeting_Docs?csf=1&web=1&e=yUFgq7)

# Genomics Invoicing

Our objective was ...

What we did as a group was ...

How far we got was ...

## Key links
- Final presentation video
- FInal presentation slides
- Link to individual learning plans
- Link to technical diaries
- Link to Github repos

# REDMANE Demo
The objective of my internship was to **revive and modernize REDMANE**, a modular Research Data Management (RDM) platform designed to help researchers securely manage, organize, and share biomedical datasets. The aim was to restore its functionality, improve stability, and prepare the system for future scalability and integration.

What I did was focus on **rebuilding the system infrastructure** by setting up and configuring the cloud environment, containers, and network layers to ensure stable communication across services. I worked on **migrating the database system** and successfully **connected the database to the backend**, improving backend functionality and deployment reliability. I also streamlined the setup process and created **comprehensive technical documentation** to support future maintenance and development.

How far I got was a **nearly complete system**, with the backend and database fully connected and running smoothly, and the final step being to establish the connection between the backend and frontend. This progress laid the groundwork for completing the full data flow and advancing REDMANE toward a production-ready stage.

## Key links
- [Final presentation video](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/EW6eFphhisNErQ19JXVJnfQBxMrnwGJcOGczOMBGfVqZRg?e=KNxu34)
- [Final presentation slides](https://wehieduau.sharepoint.com/:p:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/Semester%202%202025/Data%20Registry/REDMANE%202025S2.pptx?d=wf821941c6ff344f884624a86e8cdc29c&csf=1&web=1&e=9fBUeW)
- [Link to daily technical diary](https://wehieduau.sharepoint.com/:b:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/Semester%202%202025/Data%20Registry/Minghan%20Li%20REDMANE%20Daily%20Notes.pdf?csf=1&web=1&e=KbR9eq)
- [Link to Github repo](https://github.com/theBEST-git/REDMANE_Demo_2025s2)
- [Link to REDMANE VM Setup Guide](https://wehieduau.sharepoint.com/:b:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/Semester%202%202025/Data%20Registry/REDMANE%20VM%20Setup%20Guide.pdf?csf=1&web=1&e=1iaqN2)
- [Link to Database Migration Notes (SQLite to PSQL)](https://wehieduau.sharepoint.com/:b:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/Semester%202%202025/Data%20Registry/SQLite%20to%20PostgreSQL%20Migration.pdf?csf=1&web=1&e=NHwlKd)
- [Link to FastAPI+PSQL Setup Guide](https://wehieduau.sharepoint.com/:b:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/Semester%202%202025/Data%20Registry/REDMANE%20FastAPI%20Setup.pdf?csf=1&web=1&e=GejO3b)

# REDMANE Web Dev
The objective of our team this semester was to turn the REDMANE Data Registry into a **functional MVP** that could be shown to stakeholders. We aimed to remove hardcoded content, make pages responsive, and connect the frontend to the PostgreSQL database.

This internship, we completed three core features. **Creating new datasets, a project summary page, and uploading file metadata.** As well as updating the files view page for a dataset to be responsive, and filter between raw / processed / summarised files. The datasets and projects are now also read from the database. These features all interact directly with the database and now allow for basic Create and Read functionality (no Update and Delete just yet) in the demo.

This intake we were able to turn what was previously a basic framework for REDMANE, into a functional demo built with core create / upload features, with some advanced features still in progress, paving the way for future development.

## Key links
- [Semester 2 2025 Folder](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=pDcIAg&CID=96eb9bc2%2D2476%2D442d%2Dbb04%2D3562dbd82c60&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069&id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FData%20Commons%2F2025%20Semester%202%20Web%20Dev)
- [Final presentation video](https://wehieduau-my.sharepoint.com/personal/mosbergen_r_wehi_edu_au/_layouts/15/stream.aspx?id=%2Fpersonal%2Fmosbergen%5Fr%5Fwehi%5Fedu%5Fau%2FDocuments%2FRecordings%2FREDMANE%20Web%20Final%20Presentation%2D20251017%5F130758%2DMeeting%20Recording%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E5516915a%2Dc2bf%2D4002%2D91b4%2D147cb14d9d9f&ga=1)
- [Final presentation slides](https://wehieduau.sharepoint.com/:p:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc.aspx?sourcedoc=%7B8B397EA8-4FB4-4765-A4C2-B7F7E689A10A%7D&file=2025_Sem2Presentation.pptx&action=edit&mobileredirect=true)
- [Link to individual learning plans](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FData%20Commons%2F2025%20Semester%202%20Web%20Dev%2FIndividual%20Learning%20Plans&viewid=afd55542%2D8e3a%2D4327%2D95f9%2D63450ae10d2a&csf=1&web=1&e=pDcIAg&CID=96eb9bc2%2D2476%2D442d%2Dbb04%2D3562dbd82c60&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069)
- [Link to technical diaries](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FData%20Commons%2F2025%20Semester%202%20Web%20Dev%2FTechnical%20Diaries&viewid=afd55542%2D8e3a%2D4327%2D95f9%2D63450ae10d2a&csf=1&web=1&e=pDcIAg&CID=96eb9bc2%2D2476%2D442d%2Dbb04%2D3562dbd82c60&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069)
- [Link to Github Frontend ReactJS Repo](https://github.com/WEHI-RCPStudentInternship/REDMANE_react.js/tree/13-semester2_2025)
- [Link to Github Backend FastAPI Repo](https://github.com/WEHI-RCPStudentInternship/REDMANE_fastapi/tree/13-2025-Semester-2)
- [Link to Github Database Setup PostgreSQL Repo](https://github.com/WEHI-RCPStudentInternship/REDMANE_fastapi_public_data/tree/sem_2_2025)

# Student Organiser
### Objective

The objective of our project was to improve the **Student Organiser** application to support Rowland in managing interns, projects, and intakes more effectively. Additionally, our team aimed to design a new **Student Engagement** feature that would allow Rowland to track attendance, questions asked, and overall engagement throughout each internship period.

### What We Did as a Group

As a team, we began by reviewing the existing system, including documentation and previous interns’ work, to fully understand its workflow and current limitations. We identified several areas for improvement and prioritised features that would enhance usability, data accuracy, and supervisor efficiency.

## Our key contributions included:

- **Enhancing project and capacity management:** Implemented functionality that allows Rowland to view offered and accepted students together, providing a clearer overview of project capacity.

- **Improving project job description management:** Developed a feature that enables reuse and editing of project job descriptions for new intakes.

- **Streamlining intake management:** Added the ability to modify intake start dates and send emails directly to interns using saved templates, improving communication and reducing manual work.

- **Designing a Student Engagement system:** Created a database schema and UI layout to track student participation, including attendance records, questions asked, and communication history. This design will form the foundation for future development and integration.

- **Collaboration and testing:** Regularly held team meetings to review code, identify missing functions (such as email handling in intake management), and maintain consistency through GitHub workflows.

### Final Status

By the end of the internship, the team had successfully implemented and tested the new features for **project capacity tracking, job description management**, and **intake communication** using automated email templates.

The **Student Engagement** system was fully designed, with both the database structure and UI prototypes completed, but not yet implemented. This provides a clear and well-documented roadmap for future interns to continue building upon.

Overall, the Student Organiser is now more user-friendly, efficient, and aligned with the supervisor’s needs, setting a strong foundation for future improvements in intern management and engagement tracking.
## Key links
 [Final presentation video](https://wehieduau-my.sharepoint.com/personal/mosbergen_r_wehi_edu_au/_layouts/15/stream.aspx?id=%2Fpersonal%2Fmosbergen%5Fr%5Fwehi%5Fedu%5Fau%2FDocuments%2FRecordings%2FStudent%20Organiser%20Final%20Presentation%20Sem%202%202025%2D20251020%5F161255%2DMeeting%20Recording%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E1052496f%2D5949%2D4237%2Da8b8%2D5a3f18e216ba&ga=1)
- [Final presentation slides](https://www.canva.com/design/DAGz8areWv0/I5qfmPocTYP1-jN4NJAaqg/edit?utm_content=DAGz8areWv0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
- [Link to daily technical diary](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Student%20Organiser/2025%20S2/Daily%20Technical%20Diary?csf=1&web=1&e=uIK8Ma)
- [Link to individual learning ](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Student%20Organiser/2025%20S2/Individual%20Learning%20Plans?csf=1&web=1&e=0AEwNj)
- [Link to Github repo](https://github.com/WEHI-RCPStudentInternship/student-intern-organiser)
- [Link to Semster 2 2025](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Student%20Organiser/2025%20S2?csf=1&web=1&e=hj1aiW)
