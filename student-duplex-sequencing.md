# Duplex Sequencing Plugin Student Intern Project

## Introduction 

We are looking for interns to help us streamline quality control plot generation for duplex sequencing data.   

Duplex sequencing is a short-read sequencing technology that uses a barcoding approach to create highly accurate consensus sequences. This technology has application in diverse fields such as tumour evolution, metagenomics, forensics, ageing, and antimicrobial resistance.  

Due to the specialised nature of the technology, typical QC metrics from short-read sequencing are of limited use. Instead, we look at highly specialised metrics to determined the quality of the experiment. Currently, these metrics are calculated outside of our in-house duplex pipeline and involve running custom R scripts.  

To make the metrics easier to generate and view for the end-user, duplex-specific metrics could be generated automatically as an integrated report from the duplex processing pipeline. The current in-house duplex pipeline generates MultiQC metrics for read quality, as well as a report after consensus calling. These reports, however, are missing the more specialised duplex metrics that are utlimately the most important QC measure. 

The task for this project would be to streamline the generation of duplex specific metrics and consolidate them into the MultiQC report generated after consensus calling. A MultiQC plugin could be developed to aid in the display of duplex metrics and would be integrated into our in-house pipeline, and potentially into other open-source pipelines such as nf-core's fastquorum, which is also able to process duplex data. This would allow any duplex sequencing experiments done at the institute, and potentially outsode of the institute, to be more streamlined, and allow researcher to interpret the duplex sequencing quality more easily.  

We have data generated on E-coli, so we will be able to provide this data for testing. An [example of these plots (metric comparison plots) can be seen here](https://wehigenomicsrnd.github.io/G000204_duplex/ecoli_K12.html). 

In this role, you will need to review, curate, and build on the knowledge provided in the wiki, add your own technical notes into the Sharepoint, communicate you and your team’s progress via email on a regular basis, and turn up to online meetings.  This will help future students improve their onboarding in the future. 

## Duties while on placement 

The Research Software Engineer (Duplex Sequencing Workflows) Intern role will: 
- Connect with researchers to identify their needs  
- Review the options available for building software or workflows that fits researcher needs 
- Implement, write, and test software to ensure it is fit-for-purpose 

There is also a fair amount of flexibility with this project to allow the student to inject their own ideas and introduce new features and functionality.  


## Skills and Pre-requisites 

Skills and Pre-requisites: 
- Basic knowledge/awareness of, or ability to learn quickly one or more of the following R, Python, Nextflow, and Linux command-line 
- Ability to learn and understand high-level concepts quickly 
- Ability to work independently and to report to a group and discuss theories and results 
- Good analytical skills 
- Working with git would be an advantage 
- Understanding of general biology or bioinformatics background would be an advantage   

## Benefits for students 

Benefits for students whilst undertaking the internship include: 
- Each student will get hands on experience in working in an emerging research software environment within a highly regarded medical research institute. 
- Gain understanding of how real-world software is assessed, developed and how priorities and requirements are established within a research environment. 
- Gain understanding of the importance of maintainable, scalable and extensible code. 
- Improving oral and written communication skills in a team environment.

## Further reading
- [Duplex Sequencing from Wikipedia](https://en.wikipedia.org/wiki/Duplex_sequencing)
