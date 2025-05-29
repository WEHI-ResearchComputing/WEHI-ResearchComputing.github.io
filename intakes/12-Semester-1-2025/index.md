# RCP Internship Program - Intake 12 - Semester 1 2025

This is the list of projects for this intake. Here you will see:
- Summary of the problem and the work done in the project
- Links to the final presentation slides and/or video for the project
- Links to the github repos that were part of this project
- Links to the data needed to run the software
- Links to other documentation, such as technical diary and other project documentation.
- Links to the project management tool with the tasks shown

These reports are written by the group to help share information to future interns and interested parties.

For more examples, see the [Intake 11 - Summary Report Page](https://wehi-researchcomputing.github.io/intakes/11-Summer-2024-2025/)

# **REDMANE Data / Clinical Dashboards**

Our team's work can be broken down into 2 main parts:

### **Metadata generation for data ingestion**

*From the Summer 24/25 Data Ingestion Intake’s summary report: The challenge that we were trying to solve was ensuring that metadata uploaded to the REDMANE data registry and data portals were formatted in standardised ways. Different points of data ingestion required different metadata formats. Each data portal has its own specific format for metadata, and without a streamlined way to generate these metadata files, users would struggle to verify and upload their data correctly. This lack of consistency could lead to errors in data ingestion and disorganisation in REDMANE’s database.*

More specifically, previous scripts could only work for the files associated with only one sample, so we needed to develop and modify scripts that can extract metadata for counts.csv/.tsv files, which are associated with multiple samples. 

We solved the issue that the scripts cannot handle the counts.csv/.tsv files including multiple samples. First, we updated sample\_metadata.json from the previous intake to expand more sample ids to mimic the scenario where one patient has multiple samples. We generated 2 RNA-seq counts.csv datasets based on the mapping information in sample\_metadata.json. Second, we modified the scripts from the previous intake to suit the file types containing multiple samples (update\_local\_v1.py). At last, we optimized a script for HTML report generation, which is for the visual check on the format of Ro-Crate JSON file for data registry updates.

### **Creating synthetic databases**

Data management is the process of collecting, storing, organising, and using data in a structured manner to ensure accuracy, completeness, and security. It involves all aspects of managing data throughout its lifecycle, from creation to deletion or archiving. Essentially, it's about making sure data is accessible, reliable, and used effectively to support operations and decision-making.

Data management becomes really difficult to achieve in a scenario where the research data is spread across multiple organisations, is multi-omics (genomics, transcriptomics, proteomics, and metabolomics) in nature, and is being published through different journals. To add more complexity to this, there are different versions/stages of the data files (raw, processed, summarised) throughout the data lifecycle, and ingesting the data into the essential workflows becomes all the more complex.  

**RE**search **D**ata **M**anagement and **AN**alysis **E**nvironment (REDMANE) is a data management and analysis platform that was introduced to resolve these complex issues.

REDMANE resolves these issues by having the following features:

* Lightweight and flexible ecosystem  
* Doesn't need organisational buy-in  
* Cheaper to run than a full cloud solution  
* Easily handles new data types  
* Focused on importing information quickly and easily  
* Single Sign On  
* Can handle cross-organisation data easily

REDMANE supports different types of datasets, for example, the Whole Genome Sequencing (WGS), Single Cell RNAseq, imaging dataset, and so on. 

In this Summer 2025 intake, I narrowed down the problem space to creating an MVP to generate synthetic data for the different file types (raw, processed, and summarised) for the WGS dataset and creating a workflow to upload the corresponding metadata file to a synthetic data storage portal inspired from the cBioportal.

Through this project, we learned the importance of clear communication, collaboration and a high-level understanding of the project before diving into the tasks through asking questions. By the end of the intake, we were more equipped to break down complex and ambiguous projects, maintain documentation and effective team coordination. We also gained an understanding about research workflows and data complexity, as well as how this affects users needs. 

## **Key links**

* [Final presentation slides](https://www.canva.com/design/DAGmk8jJWs8/McJQ3Z1PEb9-i0nG9tiXXw/edit).
* [Final presentation video](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/Eb23Na3dmCRKtY_jc2NRu6YBpDs7VFKkqrNKXxjKgCYmsg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=feUsNv)  
* Github repositories:   
  * [REDMANE metadata generator with rocrate](https://github.com/lara-pawar/REDMANE-metadata-generator-with-RO-Crate)  
  * [Clinical Informatics Collaborative \- \`generatervis\`](https://github.com/Clinical-Informatics-Collaborative/generatervis)  
  * [Clinical Informatics Collaborative \- data\_storage\_portal](https://github.com/Clinical-Informatics-Collaborative/data_storage_portal)  
      
* Technical Diary  
  * [REDMANE Data Technical Notes](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20\(Data%20ingestion\)/REDMANE%20Data%20Technical%20Notes.docx?d=w69cc04a50ea4447182b37c3b7846f5f0&csf=1&web=1&e=nDJYhk)  
  * [Team Weekly Notes](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20\(Data%20ingestion\)/REDMANE%20Data%20Semester%201%20-%20Weekly%20Notes.docx?d=w171d06a97ff449e2807c62ff8d098229&csf=1&web=1&e=egsLNO)  
* [REDMANE Component Responsibility](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201/REDMANE%20Component%20Responsibility.xlsx?d=wdcae9e112c724a00a9f18305cb56c86a&csf=1&web=1&e=eCZzx3)   
* [REDMANE Document Registry](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/REDMANE%20Document%20Registry.xlsx?d=w4b032f48c70f422eadc5fd1477500dc3&csf=1&web=1&e=de8A8Y)  
* [Other useful links](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20\(Data%20ingestion\)/Relevant_links.xlsx?d=w80a4cd823f5446c3abf121ffb7f2c13c&csf=1&web=1&e=DMo1Ie)


# **REDMANE Data Curation**

The challenge we were trying to solve was how to make the process of navigating and curating complex medical data more intuitive and efficient for researchers. In medical research projects, a single patient can contribute to multiple datasets or projects, a sample may be linked to several files, and some files may not have a known dataset, often referred to as orphan files. These overlapping relationships between entities such as patients, samples, files, projects and datasets make it difficult to extract meaningful insights or organise information accurately.

The way we tried to solve this was by designing a user-friendly wireframe prototype that supports dynamic filtering, personalised dataset creation, and better visibility into the relationships across data sources. The interface was created to help users easily select and organise data based on specific criteria, identify orphan files, and even generate new logical datasets across multiple existing ones. This design lays the foundation for an interactive data curation tool that helps researchers to manage complex datasets with clarity and control.

We learned how complex medical data can be, especially when it spans across multiple projects, datasets, files, and collaborating organisations. Understanding the intricate relationships between these entities is essential, as improper data handling or mislabeling can significantly impact research outcomes, something that must be avoided in the medical field where accuracy is critical. We also recognised the importance of proper data curation practices to ensure integrity and usability.

In addition, we learned how to collaborate effectively as a team, especially in remote settings where communication is often delayed and requires more effort. We developed skills in managing distributed teamwork, asking the right questions early, and staying aligned on goals. Specifically for this project, we learned how to shape and propose a solution even when the problem is not clearly defined, focusing instead on building a platform that supports and simplifies the user's workflow.

## **Key links**

* [Final presentation slides](https://www.canva.com/design/DAGmk8jJWs8/McJQ3Z1PEb9-i0nG9tiXXw/edit).  
* Technical Diary  
  * [REDMANE Data Technical Notes](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20\(Data%20ingestion\)/REDMANE%20Data%20Technical%20Notes.docx?d=w69cc04a50ea4447182b37c3b7846f5f0&csf=1&web=1&e=nDJYhk)  
  * [Team Weekly Notes](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20\(Data%20ingestion\)/REDMANE%20Data%20Semester%201%20-%20Weekly%20Notes.docx?d=w171d06a97ff449e2807c62ff8d098229&csf=1&web=1&e=egsLNO)  
  * [Data curation notes.](https://docs.google.com/document/d/1zOAC5G0brw4F6L3env3CkMxyvNpzRKb3wECMupytFjY/edit?usp=sharing)  
  * [Data curation interfaces \- miro](https://miro.com/app/board/uXjVIChoK34=/?share_link_id=27653201771)

# REDMANE Demo

REDMANE Demo and Quality
The objective was to assess the REDMANE demo setup to identify which components were operational and which required fixes. The environment spanned five virtual machines, each hosting components like the data registry, OMERO, cBioPortal, and authentication services. Ensuring consistent configuration and accessibility was crucial for maintaining a stable testing environment.

The team reviewed six key components, focusing on service accessibility, configuration, and operational status. While some services were functional, others had issues such as missing SSL, incomplete database setups, and failed startups.

To address these issues, UptimeRobot was implemented to monitor service status in real time. A public dashboard was created for ongoing monitoring and quick issue detection.

Testing involved synthetic datasets, including Whole Genome Sequencing (WGS) data and OMERO image data, exposing further configuration conflicts in Docker and Nginx. The Docker setup was adjusted to resolve port conflicts, and Nginx was reconfigured to handle SSL connections more effectively, improving security and data transfer reliability.
The review process underscored the importance of maintaining clear documentation, particularly when multiple teams were involved in deploying and testing components across shared VMs. Creating a centralized dashboard provided a single reference point for service status, improving coordination and reducing troubleshooting time.


## Key links
- [Synthetic WGS Data Creation](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20Demo/Synthetic%20wgs%20Data%20creation.docx?d=wd9c4e2e103994ce68a5516d94b152af1&csf=1&web=1&e=VMm4M8)
- [REDMANE Component Responsibility.xlsx](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201/REDMANE%20Component%20Responsibility.xlsx?d=wdcae9e112c724a00a9f18305cb56c86a&csf=1&web=1&e=NvSRVd)
- [UptimeRobot: Demo Environment Monitoring Setup](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20Demo/UptimeRobot.Demo%20Environment%20-%20Service%20Monitoring%20Inventory.docx?d=w935ea731dbee402989f0e782f79f13ee&csf=1&web=1&e=mDoJ6y)
- [REDMANE Document Registry.xlsx](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/REDMANE%20Document%20Registry.xlsx?d=w4b032f48c70f422eadc5fd1477500dc3&csf=1&web=1&e=P308d0)
- [REDMANE Demo Technical Note: Eby](https://wehieduau.sharepoint.com/:w:/r/sites/studentinterngroupatwehi/_layouts/15/doc.aspx?sourcedoc={1ef2797f-d17f-4b20-b571-59534d6d7976}&file=redmane%20demo%20technical%20note%20eby.docx&action=default&mobileredirect=true)
- [REDMANE Demo Shared Folder](https://wehieduau.sharepoint.com/:f:/r/sites/StudentInternGroupatWEHI/Shared%20Documents/Data%20Commons/2025%20Semester%201%20Demo?csf=1&web=1&e=o5d6i7)
- [Demo and Quality Final Presentation (Semester 1, 2025)](https://unimelbcloud-my.sharepoint.com/:p:/r/personal/kkzhang_student_unimelb_edu_au/Documents/Demo%20and%20Quality%20Final%20Presentation%202025%20Semester%201%202025-05-21.pptx?d=w346a1fc51a1742688aa9a72d142fbd64&csf=1&web=1&e=lJYBHm)
- [Demo and Quality Final Presentation video](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/EayGR8rDX0ZDgesWFqacazwBgHlmN4aQr-SKBnYN487-Dg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=SUiTKy)

# REDMANE Web

Our main challenge was to was to build a fully functional, user-friendly web interface for REDMANE's data registry. We aimed to connect the backend FastAPI to the frontend React.js to enable data flow. We can then removed the hardcoded content in the frontend and replace it with dynamic data fetched from the PostgreSQL database. We also wanted to create new pages and functionalities for the data registry, including single dataset view, all files page where all the metadata for the files are stored, and creating new dataset button.

Our team took an iterative, testing-driven approach to solve the issues. First, we added synthetic data directly into the PostgreSQL database. We then verified whether this data was correctly retrieved and displayed by the FastAPI backend through its API endpoints. Only after confirming that the backend reflected the database correctly, we moved on to the frontend (React.js). We checked if the frontend was able to fetch and display the data as intended. At every stage, if the data wasn’t showing up as expected, we debugged the code—tracing the issue back through the frontend API calls, the backend routes, and the database queries. This step-by-step verification helped us ensure that the frontend was fetching data from the correct tables in the database and that the entire data pipeline was working as a cohesive system. 

When creating new pages and functionalities for the data registry, we had to think carefully about the purpose and requirements of each page. We ensured that each page’s functionality was clearly defined, and that it was properly connected to other relevant pages. For example, when creating a page for viewing single dataset details, we made sure it linked back to the dataset list page. 

We've learnt how the different components of a web application works together. How the frontend, backend, and database are connected, and how changes in one component can affect the others. This understanding helped us debug effectively and build features that integrate smoothly across the system.

In addition, we also learnt that when working with a large system like REDMANE, understanding the system architecture is essential. This made problem-solving much more efficient and strengthened our ability to trace problems across multiple layers of the system, learning how to identify whether an issue lies in the frontend, backend, or database.

## Key links
- [Final presentation slides](https://wehieduau.sharepoint.com/:p:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc.aspx?sourcedoc=%7BC32AFCDA-B950-48D0-A407-EB3CAC3F5FF0%7D&file=Presentation.pptx&action=edit&mobileredirect=true)
- [Final presentation video](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/EaiCIl3yI_hIrsgJ78kU8gQBbeihjwMm8qvlZi8Uawbt7w?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=dWob5r)
- [REDMANE FastAPI repo](https://github.com/WEHI-RCPStudentInternship/REDMANE_fastapi/tree/2025_semester_1)
- [REDMANE React.js repo](https://github.com/WEHI-RCPStudentInternship/REDMANE_react.js/tree/Semester_1_2025)
- [Web dev team technical diary](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc.aspx?sourcedoc=%7B4DBACB1D-F71F-461D-BABE-FDB6F3BD87A9%7D&file=Technical%20Diary_Eachann.docx&action=default&mobileredirect=true, https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc.aspx?sourcedoc=%7B36695DC2-4C65-4804-9245-7F7D009A1333%7D&file=Clara%27s%20technical%20diary.docx&action=default&mobileredirect=true)
- [Team Weekly Update](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc.aspx?sourcedoc=%7B14CE0193-3D97-49C5-A52D-ED069E8B10C1%7D&file=REDMANE%20Web%20Dev%20Team%20Weekly%20Update.docx&action=default&mobileredirect=true)



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
- [Multiqc and my_module.py](https://github.com/rachel610/MultiQC/tree/development/multiqc)
- [DuplexSequencingProject](https://github.com/azlan2003/DuplexSequencingProject/tree/main)
- [Duplex Sequencing Snakemake Pipeline](https://github.com/WEHIGenomicsRnD/duplex-seq-pipeline)
- [G000204_duplex](https://github.com/WEHIGenomicsRnD/G000204_duplex)

Links to the data needed to run the software
- DuplexMetricsProject - OneDrive
Links to other documentation, such as technical diary and other project documentation
- [Duplex Sequencing Plugin Student Intern Project](https://wehi-researchcomputing.github.io/student-duplex-sequencing)
- [Ecoli K12 Notebook](https://wehigenomicsrnd.github.io/G000204_duplex/ecoli_K12.html)
- [Technical Diary (Kevin)](https://docs.google.com/document/d/1ZG3tf5Uxw9GY_c4Gl9sx3Sw_4v1AWD-MM2sUOUgparw/edit?tab=t.0)
- [WEHI sharepoint folder](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=csSHFK&CID=b8e7e010%2D3ec4%2D45d1%2Db4ef%2D1722864d7b33&FolderCTID=0x0120008FF8F20683AC284798EA496C639CC069&id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FDuplex%20Sequencing)
- [Pipeline Schematic](https://www.canva.com/design/DAGiIPIb1gY/rj2FNR1Vh1tDmmopFOAgvQ/edit?utm_content=DAGiIPIb1gY&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

# **AIVE**

The challenge that we were trying to solve was to streamline dataflow within ParaView software. Most of the functions were performed manually on ParaView, which meant users had to manually import and export files, and individually apply filtering like creating contours to each mask. This repetitive work in filtering and adjusting parameters cause inefficiency when reproducing experiments in the software. Creating functions that tackle this problem requires knowledge of writing scripts and how to carefully integrate them into the software. 

To address the problem, we developed a user-friendly interface (UI) using the Tkinter toolbox in Python and adapted scripts from the Start Trace function in ParaView. This UI allows users to input specific parameters related to ParaView settings—such as folder paths, file prefixes, and isocontour values—which are then stored in a configuration file for automated processing within ParaView. The scripts have been successfully tested on the Milton High Performance Computing (HPC) system, enabling broader usability across WEHI. Additionally, complementary scripts (e.g., for exporting data as .stl files) were created to enhance user convenience and streamline the workflow.

Through this process, we learned how to write correct Python scripts and config files, build a smooth user interface, and test the robustness of our program in different environments including the HPC system. Additionally, we also learned soft skills like communication, collaboration, problem-solving, and critical thinking.

## Key links
- [Final presentation slides](https://docs.google.com/presentation/d/1lxnRx3ag-3WRUrhMkMs8SZ6hP-Eqi_uCd_Z6r9HGw7s/edit?slide=id.p#slide=id.p)
- [Links to the github repos that were part of this project](https://github.com/MitochondRuna/AIVE-Intro/tree/WEHI-Internship-S1-2025)
- [Links to the data needed to run the software](https://drive.google.com/drive/folders/1tYgeA7FHXffrVzm1vBYM-A8hfXKE_rT-?usp=drive_link)
- [Links to other documentation, such as technical diary and other project documentation ](https://github.com/MitochondRuna/AIVE-Intro/tree/WEHI-Internship-S1-2025/UI_for_Paraview_Processing/Final_Scripts)

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

The challenge that we were trying to solve was reproducibility issues in bioinformatics workflows, such that any two systems could produce the same output with the same input. Computing environments will rarely be equal amongst bioinformaticians, and so outputs on the same software will also tend differ between individuals. A multitude of factors can contribute to this – inclusive of (but not limited to) system configurations and dependency updates or version mismatch – and as such a solution calls for unification of workflows under one consistent environment umbrella. This is the BioNix project at its core, improving upon or otherwise reinforcing reproducibility in existing bioinformatics tools under Nix to maintain repeatable outputs.

The way we tried to solve this was by utilising Nix, a declarative, functional package manager built from the ground up for reproducibility and reliability. In short, Nix ensures reproducibility by building packages using only the specified dependencies (and dependency versions) in complete isolation from each other. The main crux of our project focussed around the VIRUSBreakend software, more specifically, its dependencies of Kraken2 and RepeatMasker. We developed derivations of these dependencies in Nix, wrapping and shipping them to nixpkgs, an open-source repository of packages.

Through this process, we learned how to Nix, constructing wrappers for software that benefit greatly from reproducibility. We developed an appreciation for the high-level concepts and functions of the system, and were able to understand the importance of this knowledge when tackling difficult problems. We continuously faced open-source norms towards the end of the project, and so constructing a solid grasp on how we should tailor our work for integration into a public repository such as nixpkgs was also incredibly useful.


## Key links
- Final Presentation (to be added):
  > Slides
  >
  > Video
- Whiteboard Presentations:
  > Sem 1 2025 (tba)
  >
  > [Sem 2 2024](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/_layouts/15/stream.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FBioNix%20Introduction%2FWhiteboard%20Presentation%20%2D%20BioNix%20%2D%20Semester%202%202024%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E6ee65d0f%2D3d96%2D4efe%2Db2cb%2D2eacaeb6aadb)
- Repositories:
  > [BioNix](https://github.com/PapenfussLab/bionix)
  >
  > [GRIDSS (VIRUSBreakend)](https://github.com/PapenfussLab/gridss)
  >
  > [nixpkgs](https://github.com/NixOS/nixpkgs)
  >
  > [Semester 1 2025 Intake Repository](https://github.com/cardealerT/intern_repo)
- Previous Intake Presentations
  > [Semester 2 2024](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/_layouts/15/stream.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FBioNix%20Introduction%2FFinal%20Presentation%20Semester%202%202024%20BioNix%2D20241008%5F093501%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E505ccfaf%2Dd8b4%2D4628%2Dbb4d%2D5f6b1a904041)
  >
  > [Summer 2023-2024](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/_layouts/15/stream.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FBioNix%20Introduction%2FFinal%20Presentation%20Summer%202022%202023%20BioNix%20Lezhou%20and%20Daniel%20Student%20Presentations%2D20230223%5F123238%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E379ee374%2Dcc29%2D469b%2Da378%2Dc9ce638fc541)
  >
  > [Semester 2 2022](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/_layouts/15/stream.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FBioNix%20Introduction%2FFinal%20Presentation%20Semester%202%202022%20BioNix%20Kai%20Bing%20Bionix%20Student%20Presentations%2D20221124%5F142758%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E3beced9b%2Dfe48%2D438d%2Dbbb1%2D5fb93c9d35f2)

# Student Organiser

**Challenge Statement**

The challenge we were trying to solve was improving the usability and efficiency of the WEHI Student Intern organiser Web app, specifically focusing on managing project allocation and streamlining recruitment and onboarding processes. The existing system required manual updates and lacked interactive features, making it time-consuming for team members to manage project status and track intern progress.

**Approach and Solution**

The way we approached this challenge was by first gaining a high-level understanding of Rowland’s workflow and identifying the key pain points, especially around project allocation and managing weekly updates. Our team worked collaboratively to develop solutions that addressed these issues while maintaining compatibility with the existing system. After understanding Rowland’s overall workflow and the problems he faced, we started on working on the web app. First, we fixed the database off bugs so that it aligns with the UI features we want to implement. We also made some sample data that can be easily used for web app testing purposes even for future interns. Next, we enhanced the project allocation page by making status management easier, adding data visualisation, and improving user interface. Lastly, we made a student reminder page used to track student’s submission and remind them when necessary.

Throughout the project, we worked closely as a team to align database updates with the new UI features, ensuring consistency between the backend and the frontend. Regular communication with Rowland helped us incorporate his feedback and make iterative improvements. These made project management more intuitive and efficient

**Key Learnings**

We learned that successful software improvements require balancing technical solutions with user-centric design. Understanding high-level goals and incorporating feedback were crucial to ensuring that the changes were both functional and practical. Additionally, we gained valuable experience in collaborating effectively within a multidisciplinary team, maintaining clear communication, and prioritizing user needs throughout the development process.



## Key links
- [Final Presentation Student Organiser.pptx](https://wehieduau.sharepoint.com/:p:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc2.aspx?action=edit&sourcedoc=%7B6da65a83-3de1-4365-8712-644c8b32d6a3%7D&wdOrigin=TEAMS-MAGLEV.teamsSdk_ns.rwc&wdExp=TEAMS-TREATMENT&wdhostclicktime=1748482054051&web=1)
- [Final Presentation Video Link](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/EcSmGoOfruVPmD9AXMMFxCwBV2ou6DIxa9cbe60_pTMbLw?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=KteWEI)
- [Student organiser Wiki link](https://github.com/WEHI-RCPStudentInternship/student-intern-organiser/wiki)
- [Student Organiser Github Link](https://github.com/WEHI-RCPStudentInternship/student-intern-organiser)
- [Understanding of Rowland's Workflow.xlsx](https://wehieduau.sharepoint.com/:x:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc2.aspx?action=edit&sourcedoc=%7B800dc76a-afff-4628-9b3c-69249bcbced0%7D&wdOrigin=TEAMS-MAGLEV.teamsSdk_ns.rwc&wdExp=TEAMS-TREATMENT&wdhostclicktime=1748481928717&web=1)
- [Internship weekly update.docx](https://wehieduau.sharepoint.com/:w:/r/sites/StudentInternGroupatWEHI/_layouts/15/Doc2.aspx?action=edit&sourcedoc=%7Bb3573169-f62d-47ff-81b5-7919e7a6bdda%7D&wdOrigin=TEAMS-MAGLEV.teamsSdk_ns.rwc&wdExp=TEAMS-TREATMENT&wdhostclicktime=1748481831783&web=1)


# RAG LLM

One of the existing problems with the onboarding process for the internship is that our supervisor is handling 38 interns by himself and he would receive repeated questions from students. Another problem we are solving is the difficulty in finding answers to a question due to the large number of existing WEHI websites, resources and documentation. Although the previous intake has built a chatbot that is functional, the accuracy is at 75% which may cause distrust in the user, and they may avoid using the system. Ultimately, interns will resort back to asking the supervisor questions.  

Hence, due to RAG LLM’s inconsistent results, we focused on finding strategies to improve the trust of a user in the chatbot system. We attempted to solve this by implementing a system that allows users to choose different search methods (keyword, semantic and RAG LLM) to receive an answer to their queries. We also incorporated extra mechanisms to enhance the system, such as logging all queries and answers for our supervisor to track. Additionally, as the previous intake provided two sets of architecture for the chatbot, we experimented and decided on an architecture that combines the two, taking the best from both within computational limits.  

We have learned how to build a versatile architecture by making each of layer of the architecture independent. Doing so, we can interchange the search methods without needing to build a new architecture. Besides that, we have learned how to prioritize tasks effectively to ensure that we achieve as much as we can in the short time frame. For instance, we have decided to use a third-party template for user interface to reduce the time spent on that component to focus on enhancing the accuracy of the chatbot. 


## Key links
**Final Presentation:** 
- [2024/25 Summer Intake Final Presentation](https://wehieduau.sharepoint.com/sites/StudentInternGroupatWEHI/_layouts/15/stream.aspx?id=%2Fsites%2FStudentInternGroupatWEHI%2FShared%20Documents%2FStudent%20Organiser%2FFinal%20Presentation%20RAG%20LLM%2020250218%5F093045%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Ecec5ab88%2D2105%2D48e6%2Dbe92%2Ddd10e9901451)
- [2025 Semester 1 Intake Final Presentation Video](https://wehieduau-my.sharepoint.com/:v:/g/personal/mosbergen_r_wehi_edu_au/EfqzC8Fi33BDomqAP_A1AQABWLoqyuCT3e18tYLZt6FNSA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=MyeMLz)
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
