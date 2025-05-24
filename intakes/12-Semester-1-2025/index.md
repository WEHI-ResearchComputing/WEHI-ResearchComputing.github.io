# RCP Internship Program - Intake 12 - Semester 1 2025

This is the list of projects for this intake. Here you will see:
- Summary of the problem and the work done in the project
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

These reports are written by the group to help share information to future interns and interested parties.

For more examples, see the [Intake 11 - Summary Report Page](https://wehi-researchcomputing.github.io/intakes/11-Summer-2024-2025/)

# REDMANE Data / Clinical Dashboards

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

# REDMANE Demo

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

# REDMANE Web

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown


# Duplex Sequencing

The challenge that we were trying to solve was to streamline an existing pipeline to support the visualisation of Duplex Sequencing metrics, specifically using E.coli K12 data as a case study. This involved several key challenges:  
Streamlining existing pipelines to reduce complexity, improve maintainability, and support reproducible QC reporting.
Integrating external R scripts that were under a GPL license into the pipeline which is under an MIT licence.
Maintaining flexibility to allow researchers to incorporate desired specialised metrics into the final report.

The way we tried to solve this was …
Modularising the pipeline by splitting the current pipeline into more manageable steps, the R scripts to undergo the calculations and the MultiQC plugin to output plots:
R-script: 
Separating the R code into scripts allowed us to process the rinfo files and produce a long-format output that can be easily consumed in downstream reporting such as MultiQC. To address licensing issues, we containerised the rscripts using Docker. This ensures the NanoSeq code remains encapsulated and allows future users to interact with the container without needing to modify the R codes. 
MultiQC:
Creating a MultiQC plugin enables the generation of MultiQC plots from summary data, but also facilitates the creation of custom plots using more specialised duplex specific metrics. The MultiQC plugin was created using Seqera documentation and Python. 

What we learned through this process …
Communicating with team members and checking in with supervisors is really important to make sure your project is on track.
How to create and run containers and use Multiqc and create Multiqc plugin
How to break down complicated and ambiguous tasks into simple and manageable components. This helped with the overall development. 

Key links
Links to the final presentation slides and/or video for the project
Final Presentation Duplex Sequencing Project.pptx
Links to the github repos that were part of this project
[Multiqc and my_module.py] (https://github.com/rachel610/MultiQC/tree/development/multiqc)
[DuplexSequencingProject] (https://github.com/azlan2003/DuplexSequencingProject/tree/main)
[Duplex Sequencing Snakemake Pipeline] (https://github.com/WEHIGenomicsRnD/duplex-seq-pipeline)
[G000204_duplex] (https://github.com/WEHIGenomicsRnD/G000204_duplex)
Links to the data needed to run the software
DuplexMetricsProject - OneDrive
Links to other documentation, such as technical diary and other project documentation
[Duplex Sequencing Plugin Student Intern Project](https://wehi-researchcomputing.github.io/student-duplex-sequencing)

[Ecoli K12 Notebook](https://wehigenomicsrnd.github.io/G000204_duplex/ecoli_K12.html)

[Technical Diary (Kevin)](https://docs.google.com/document/d/1ZG3tf5Uxw9GY_c4Gl9sx3Sw_4v1AWD-MM2sUOUgparw/edit?tab=t.0)

[WEHI sharepoint folder](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=csSHFK&CID=b8e7e010%2D3ec4%2D45d1%2Db4ef%2D1722864d7b33&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069&id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FDuplex%20Sequencing)

[Pipeline Schematic](https://www.canva.com/design/DAGiIPIb1gY/rj2FNR1Vh1tDmmopFOAgvQ/edit?utm_content=DAGiIPIb1gY&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

# AIVE

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

# Genomics Invoicing

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

# BioNix

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

# Student Organiser

The challenge that we were trying to solve was ...

The way we tried to solve this was ...

What we learned through this process ...


## Key links
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation
- Links to the project management tool with the tasks shown

# RAG LLM

One of the existing problems with the onboarding process for the internship is that our supervisor is handling 38 interns by himself and he would receive repeated questions from students. Another problem we are solving is the difficulty in finding answers to a question due to the large number of existing WEHI websites, resources and documentation. Although the previous intake has built a chatbot that is functional, the accuracy is at 75% which may cause distrust in the user, and they may avoid using the system. Ultimately, interns will resort back to asking the supervisor questions.  

Hence, due to RAG LLM’s inconsistent results, we focused on finding strategies to improve the trust of a user in the chatbot system. We attempted to solve this by implementing a system that allows users to choose different search methods (keyword, semantic and RAG LLM) to receive an answer to their queries. We also incorporated extra mechanisms to enhance the system, such as logging all queries and answers for our supervisor to track. Additionally, as the previous intake provided two sets of architecture for the chatbot, we experimented and decided on an architecture that combines the two, taking the best from both within computational limits.  

We have learned how to build a versatile architecture by making each of layer of the architecture independent. Doing so, we can interchange the search methods without needing to build a new architecture. Besides that, we have learned how to prioritize tasks effectively to ensure that we achieve as much as we can in the short time frame. For instance, we have decided to use a third-party template for user interface to reduce the time spent on that component to focus on enhancing the accuracy of the chatbot. 


## Key links
**Final Presentation:** 
- [2024/25 Summer Intake Final Presentation](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/_layouts/15/stream.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FStudent%20Organiser%2FFinal%20Presentation%20RAG%20LLM%2020250218%5F093045%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Ecec5ab88%2D2105%2D48e6%2Dbe92%2Ddd10e9901451)
- [2025 Semester 1 Intake Final Presentation]
- [2025 Semester 1 Intake Final Presentation Slides](https://wehieduau.sharepoint.com/:p:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/RAG%20LLM/2025%20Semester%201%20Intake/Final%20Presentation.pptx?d=wbd487bc7223d457481261d6409e5895f&csf=1&web=1&e=7cia1Q)

**Github:** 
- [2024/25 Summer Intake - Aaron](https://github.com/aaronlai-dev/student-organiser-rag-llm)
- [2024/25 Summer Intake - Arezoo](https://github.com/arzmos/student-organiser-rag-llm)
- [2025 Semester 1 Intake](https://github.com/ashleycjwork/sem1-25-student-organiser-rag-llm)

**Technical Diaries:** 
- [Technical Diary (Ashley)](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/RAG%20LLM/2025%20Semester%201%20Intake/Ashley%20Technical%20Diary.docx?d=wa134dcf226af429dba54e48b318832ea&csf=1&web=1&e=ue7OYF)
- [Technical Diary (Olivia)](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/RAG%20LLM/2025%20Semester%201%20Intake/Olivia%20Technical%20Diary.docx?d=w2fdda3159fd044a49d4cbf810b92a7a8&csf=1&web=1&e=6C9AcA)

**Project Management:** 
- [Project Tracker](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/RAG%20LLM/2025%20Semester%201%20Intake/Project%20Timeline.xlsx?d=w9c8f816e70c64c808cda417dfb1e8f62&csf=1&web=1&e=p6Rivk&nav=MTVfezAwMDAwMDAwLTAwMDEtMDAwMC0wMDAwLTAwMDAwMDAwMDAwMH0)

# To update this file

Go to [Github and fork this repo, make changes, and then do a pull request back to the original repo. This is the file you need](https://github.com/WEHI-ResearchComputing/WEHI-ResearchComputing.github.io/tree/main/intakes/12-Semester-1-2025/index.md).
