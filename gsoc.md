# Google Summer of Code Project List

This is a list of projects we are submitting to the Google Summer of Code for 2022.

To apply, you can [read our suggestions for applying](gsoc-contributor) to these roles.

# General Projects

## BioNix - Research Software Engineering

This project would suit a candidate who was interested in reproducibility, wants to gain experience with executing bioinformatics workflows efficiently, and enjoys streamlining complex processes.

Bioinformatics as a discipline frequently uses many individual software tools, connected in potentially complicated ways, to perform typical analysis. As an example, standard Single Nucleotide Variant (SNV) calling in cancer involves alignment of the sequencing reads to a reference genome, sorting and indexing, variant calling, and subsequent annotation against various databases. Each of these stages comprises of one or more software tools with different input requirements. 

As a result, reproducibility is difficult to achieve due to the large number of components and the complicated dependency structure inherent in both building the software tools and execution of the workflow. A recently proposed solution to the problem, BioNix[1], leverages the Nix[2] functional package management system to both manage the software and execute the workflow. This has allowed an unprecedented level of reproducibility in the field. 

The candidate will be responsible for expressing various bioinformatics processing pipelines in the BioNix workflow framework. The goal is to write a variety of standard processing pipelines within the framework, making typical analysis both easily accessible and highly reproducible to many bioinformatics researchers. This will include: 
- wrapping underlying bioinformatics software that is required and not currently available in nixpkgs[3]; 
- writing expressions to execute the tools as individual processing stages; 
- test each stage in isolation to verify functionality and bit-reproducibility; 
- test whole workflows for functionality. 

Skills required: 

- knowledge of the use of POSIX systems; 
- understanding of version control systems, experience with git will be helpful; 
- functional programming skills, experience with Nix/NixOS will be helpful. 

References
1. https://github.com/PapenfussLab/bionix 
2. https://nixos.org/ 
3. https://github.com/nixos/nixpkgs 



---

# Image Processing Portal set of projects

Advanced microscopes are now capable of producing very large (terabyte scale) datasets in a single imaging session. Migrating, processing, quantifying and visualising these large datasets is a major bottleneck for traditional wet-lab biologists. This project will help create tools to unlock scientific breakthroughs in the fields of developmental biology, cell biology and human disease and infection, by unlocking high performance compute resources and new technologies to an untrained and naïve user audience. 


The intention of this proposal is to gain support for the continued development of a suite of open-source tools accessible to all researchers for the purpose of processing & visualising big microscopy data.  This includes establishing the IPP at various universities and institutes both in Australia and Internationally.

Below is a list of available projects for the image processing portal that will leverage existing investment and provide the tools researchers require to manage, process, quantify and visualise their large datasets. 

## Google Colab integration

This project would suit a candidate who is interested in integrating existing open-source web-based tools into a local HPC instance.

Existing image processing tools are available as Google Colab projects providing 	ease of access to challenging processing tasks such as machine learning and deep 	learning packages. This workflow is not suitable for some sensitive datasets, thus 	implementing instances of these packages within the IPP would allow for such 		workflows to be run on local hardware in adherence with funding body policy.  

The candidate would be responsible for developing both the front end interface as well as the back end integration into the HPC job scheduler. 

Skills required: 

- Knowledge of the use of POSIX systems. 
- Experience with or ability to quickly learn version control systems like git. 
- Experience with or ability to quickly learn functional programming skills and other programming skills like HTML, Nix/NixOS,and Python.  

## User Experience - Research Software Engineering

This project would suit a candidate who would like to work on front-end design and coding, and likes to learn the end-user workflow to help streamline and make the user interface intuitive. 

The unique selling point of the IPP is to make it easy for the researchers to do complex work in a simple environment that is intuitive and easy to use. This project will help to improve the UX of the IPP in a way that benefits others. 

The candidate will be responsible for developing an exceptional and intuitive user centric interface which enables researchers to effortlessly process their datasets. This will include: 
- Reviewing researcher workflows and understanding the high-level research process
- Understanding the language and nuance of how researchers currently process this Big Data
- Converting understanding into design and implementing said design in a way that is effective and efficient

Skills required:
- Experience with or ability to quickly learn web technologies such as jQuery, Bootstrap, AngularJS
- Ability to learn high-level complex concepts quickly
- Ability to work independently
- Ability to handle an ambiguous and constantly changing environment

## Fast File Converters (Read/Write) - Research Software Engineering

This project would suit a candidate who would like to work on making low-level software extremely efficient and effective within a High Performance Computing (HPC) environment. 

Existing [Bioformats file readers](https://www.openmicroscopy.org/bio-formats/) are capable of reading many microscopy related, proprietary file formats, however they are often extremely slow and are not optimised for the parallelised environment of High Performance Computing  (HPC).  

The candidate will be responsible for developing parallelized high-speed readers and writers so that we can read file formats from global vendors, process the data on the HPC, then write out to a different format, enabling fast seamless data movement between acquisition and commercial visualisation & analysis software. 

Skills required:
- Knowledge of the use of or the ability to quickly learn POSIX systems and low-level languages such as C++. 
- Knowledge of the use of or the ability to quickly learn version control systems such as git. 
- Knowledge of or the ability to quickly learn functional programming skills.
- Ability to learn high-level complex concepts quickly
- Ability to work independently
- Ability to handle an ambiguous and constantly changing environment


## Lightweight Web-based Multi-dimensional Image Viewer 

This project would suit a candidate who would like to work on combining front end web-based GUI elements with back end high speed HPC data processing tools through use of HPC job submission. 

Handling Big Data has many issues including the ability for users to quickly view n-Dimensional datasets for verification of quality and suitability for further processing.   

UQ has developed an existing tool called “Phoebe” that allows users to non-sequentially scrub through Big Data through the use of HPC resources.  This project would aim to integrate this existing tool into the IPP. 

The candidate would be responsible for developing a lightweight n-dimensional web-based image viewer, which would allow users to scrub through their files to confirm suitability for subsequent processing steps. 

Skills required: 
- Experience with or ability to quickly learn version control systems like git. 
- Experience with or ability to quickly learn functional programming skills and other programming skills like HTML, Python and C/C++. 


## Image operations

This project would suit a candidate who would like to work on developing and/or optimising existing single threaded code for parallelisation in a HPC environment and learning more about HPC job submission.

Performing common image processing tasks on Big Data is often extremely slow using desktop PCs, our goal is to move these tasks to HPC to speed up and simplify the workflow for the end user.  Simple image processing tasks such as user-defined cropping, dimensionality reduction, registration and bleach correction are often already written in various languages and packages, but often are single threaded. 

The candidate for this project would help combine these exiting open-source tools into a parallelisable, multi-threaded image processing toolbox implementation into the IPP.  

Tools to be developed may include: 
- ROI Crop Images using the lightweight image viewer  
- Maximum/Minimum Intensity Projections  
- Spherical and Chromatic aberration correction 
- Volumetric Registration & Stitching 
- 4D image arithmetic manipulations  


 Skills required: 
- Experience with or ability to quickly learn version control systems like git. 
- Experience with or ability to quickly learn functional programming skills and other programming skills like HTML, JAVA, JavaScript, Python and C/C++. 


## ImageJ/FIJI/Napari macro job submission 

This project would suit a candidate who is interested in developing skills in integrating existing open-source tools through API calls to develop a data-processing pipeline via HPC job submission. 

ImageJ/FIJI is an existing open-source image analysis tool familiar to most biologists, with a large number of active plugins and tools being developed. ImageJ/FIJI has its own macro language (IJM) and can support several other languages such as Java, JavaScript, python and Groovy. Similarly, projects are underway for this type of feature to be implemented in the modern python implementation of image processing viewers, Napari.  

This project would create a page for the Image Processing Portal where users can submit their own code to run in batch mode on their connected files. 

Skills required: 

- Experience with or ability to quickly learn version control systems like git. 
- Experience with or ability to quickly learn functional programming skills and other programming skills like HTML, JAVA, JavaScript, Python and C/C++. 


