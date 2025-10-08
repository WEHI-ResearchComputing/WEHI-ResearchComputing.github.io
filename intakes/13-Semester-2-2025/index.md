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

Our objective was ...

What we did as a group was ...

How far we got was ...

## Key links
- Final presentation video
- FInal presentation slides
- Link to individual learning plans
- Link to technical diaries
- Link to Github repos

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
