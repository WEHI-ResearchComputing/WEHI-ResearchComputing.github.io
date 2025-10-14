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

Our objective was ...

What we did as a group was ...

How far we got was ...

## Key links
- Final presentation video
- FInal presentation slides
- Link to individual learning plans
- Link to technical diaries
- Link to Github repos

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
Our objective was ...

What we did as a group was ...

How far we got was ...

## Key links
- Final presentation video
- FInal presentation slides
- Link to individual learning plans
- Link to technical diaries
- Link to Github repos

# Student Organiser
Our objective was ...

What we did as a group was ...

How far we got was ...

## Key links
- Final presentation video
- FInal presentation slides
- Link to individual learning plans
- Link to technical diaries
- Link to Github repos
