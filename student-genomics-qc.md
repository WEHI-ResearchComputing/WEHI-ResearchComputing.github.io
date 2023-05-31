# Genomics Quality Control Student Intern Project

## Introduction 
 
Post-sequencing quality control (QC) is an important step in ensuring that the quality of sequencing data meets expectations. Multiple tools exist to evaluate sequencing quality, such as FastQC[1], Fastq Screen[2] and Qualimap[3]. Core sequencing facilities, such as WEHI Genomics, process hundreds of sequencing runs every year. In order to troubleshoot sequencing issues and provide assurance of data quality to collaborators, sequencing facilities must implement robust data management workflows to ensure that QC data processing is automated where possible, is easily accessible and is appropriately archived for posterity. Given a large volume of runs, there exists the possibility of inter-run QC comparisons to better gauge run quality.  

MultiQC[4] is a software tool that collates and displays QC information from numerous supported bioinformatics tools. MultiQC operates on a per-run basis, however, MegaQC[5] collates the data from these reports for comparison. However, MegaQC has not been in active development since 2020 and is considered “pretty unstable” by the developers. Additionally, the software lacks functionality that lists extensive project metadata, so that experiments can be more easily tracked and MultiQC reports can be easily located. Lastly, the tool lacks easy exporting of data, so that analyses can be further analysed programmatically. 

Given that MegaQC overlaps with many of our use cases, it may be possible to modify and/or extend the software for our use cases. Alternatively, Shiny apps (shiny.rstudio.com) allow for interactive data analysis and provide an ideal platform for QC data collation. Integration with Monday.com and LabArchives used by the Genomics lab may also be of benefit for retrieving and/or depositing QC data and project metadata. 

1. FastQC. "FastQC: a quality control tool for high throughput sequence data." (2016). 
2. Wingett, Steven W., and Simon Andrews. "FastQ Screen: A tool for multi-genome mapping and quality control." F1000Research 7 (2018). 
3. Okonechnikov, Konstantin, Ana Conesa, and Fernando García-Alcalde. "Qualimap 2: advanced multi-sample quality control for high-throughput sequencing data." Bioinformatics 32.2 (2016): 292-294. 
4. Ewels, Philip, et al. "MultiQC: summarize analysis results for multiple tools and samples in a single report." Bioinformatics 32.19 (2016): 3047-3048. 
5. https://megaqc.info/ 


## Duties while on placement 

The Research Software Engineer Intern role will:  
- work closely with researchers to identify their needs around Genomics quality control at scale
- Review the applications available for maintainability and extensibility 
- Implement trial applications such as MegaQC to test fit-for-purpose

There is also a fair amount of flexibility with this project to allow the student to inject their own ideas and introduce new features and functionality. 

## Skills and Pre-requisites 

Skills and Pre-requisites: 
- Basic knowledge or ability to learn quickly Python/Javascript/CSS, databases and Linux command-line
- Ability to learn and understand high-level concepts quickly 
- Ability to work independently and to report to a group and discuss theories and results 
- Good analytical skills 
- Working with git would be an advantage  

## Benefits for students

Benefits for students whilst undertaking the internship include:
- Each student will get hands on experience in working in an emerging research software environment within a highly regarded medical research institute.  
- Gain understanding of how real-world software is assessed, developed and how priorities and requirements are established within a research environment. 
- Gain understanding of the importance of maintainable, scalable and extensible code. 
- Improving oral and written communication skills in a team environment. 
