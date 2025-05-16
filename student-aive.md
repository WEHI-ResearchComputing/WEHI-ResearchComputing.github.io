# Research Software Engineer (AIVE) 

## Introduction

Our cells contain a vast array of interacting organelles (tiny structures within cells that perform specific tasks, similar to the parts of a machine) that determine cellular processes through both health and disease. These structures may be imaged using electron microscopy by bouncing electrons off heavy-metal stained membranes. The resulting images have a resolution of nanometers per voxel (the 3D equivalent of an image pixel) in 3D and each data set may contain millions or billions of voxels per cell. [1] 

In a paper from 2021 [2] a new method for processing images from the focused ion beam-scanning EM (FIB-SEM) was used to image the cellular ultrastructure of phagophore-ER contacts in three dimensions. 

As per the paper: 

_FIB-SEM is ideally suited for the acquisition of 3D ultrastructural images from large cellular volumes (Hoffman et al., 2020). However, traditional methods for the reconstruction and analysis of such data require manual image segmentation and classification. The hand-drawn surfaces that are generated during manual segmentation are laborious to produce, low throughput, and subject to human imprecision, making them unsuitable for large-scale morphometric analyses. To overcome these limitations, we developed an approach that delegates the most time-consuming tasks to an artificial intelligence (AI) within a framework that captures the true surface detail of intracellular organelles. Using the machine learning capabilities of Waikato Environment for Knowledge Analysis (WEKA) in combination with ImageJ (Arganda-Carreras et al., 2017; Frank et al., 2004; Schindelin et al., 2012), we trained a random forest computer vision model to faithfully detect all cellular membranes in volumetric FIB-SEM data (Figures 6A and 6B). We have termed this 3D framework AIVE (AI-directed voxel extraction; workflow outlined in Figure S7)._

The project would involve a series of stages to bring the software infrastructure to a level that will help with development. The initial stage would involve the setup of the workflow along with testing and improving the documentation of the workflow on a local laptop. The potential second stage would be to aim to run the workflow in the WEHI HPC environment known as Milton.  

The potential third stage would be to add more data to test the workflow to ensure that the test coverage is broader than it is currently. Once this third stage is achieved, there will be an opportunity to work on streamlining the AIVE workflow. 

 

References: 

1. https://en.wikipedia.org/wiki/Electron_microscope 
2. https://www.sciencedirect.com/science/article/pii/S1097276521001696  

 

 
## Duties while on placement

In this role, you will need to be willing to read and synthesise the original paper with the latest documentation, and work with the Research Software Engineer (RSE) to help streamline all parts of the workflow. 

The Research Data Engineer Intern role will:  

- review existing semi-automated workflows that are processing FIB-SEM data, 
- test and improve documentation and regression testing for these FIB-SEM data workflows, 
- setup appropriate software development infrastructure to aid in the maintenance and improvement of FIB-SEM workflows, and 
- potentially improve the data workflow with the regression FIB-SEM data available. 

There is also flexibility with this project to allow the student to inject their own ideas and introduce new features and functionality. 


## Skills and Pre-requisites


- Interest in cutting edge image processing and AI 
- Basic knowledge of Linux command-line 
- Willingness and ability to learn and understand high-level concepts quickly 
- Ability to work independently and to report to a group and discuss theories and results 
- Good analytical skills 
- Previous experience with git would be useful but not necessary 


## Benefits for students 

The benefits for students whilst undertaking the internship include:

- Working in a High Performance Computing environment or adjacent environment. 
- Practical experience with potential exposure to Bash and Java. 
- Gain understanding of how real-world software is assessed, developed and how priorities and requirements are established within a research environment.  
- Gain understanding of the importance of maintainable, scalable and extensible code. 


## Further reading
- [Public wiki for AIVE](https://github.com/MitochondRuna/AIVE-Intro/wiki)
