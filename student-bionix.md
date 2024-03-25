# BioNix Open Source Student Internship Project

## Introduction

Bioinformatics as a discipline frequently uses many individual software tools, connected in potentially complicated ways, to perform typical analysis. As an example, standard Single Nucleotide Variant (SNV) calling in cancer involves alignment of the sequencing reads to a reference genome, sorting and indexing, variant calling, and subsequent annotation against various databases. Each of these stages comprises of one or more software tools with different input requirements. 

As a result, reproducibility is difficult to achieve due to the large number of components and the complicated dependency structure inherent in both building the software tools and execution of the workflow. A recently proposed solution to the problem, BioNix[1], leverages the Nix[2] functional package management system to both manage the software and execute the workflow. This has allowed an unprecedented level of reproducibility in the field. 

In this project, we expose you to Open Source and ask you to become an open source contributor to global open source Nix packages.

## Duties while on placement

The candidate will be get the opportunity to: 

- Learn about open source norms; 
- Improve the documentation around Nix and BioNix to make it easier and quicker to learn concepts; 
- Wrap underlying bioinformatics software that is required and not currently available in nixpkgs[3] as an open source contributor; 

Further bonus goals include:  

- writing expressions to execute the tools as individual processing stages; 
- test each stage in isolation to verify functionality and bit-reproducibility; 
- test whole workflows for functionality. 

## Skills and Pre-requisites

This project would suit a research software engineering candidate who was interested in reproducibility, wants to gain experience with executing bioinformatics workflows efficiently, and enjoys streamlining complex processes.

Skills required: 

- knowledge of the use of POSIX systems; 
- understanding of version control systems, experience with git will be helpful; 
- functional programming skills, experience with Nix/NixOS will be helpful. 

## Benefits for student

The benefits for the studnet include:
- The student will learn the basic awareness and knowledge of data reproducibility.
- Basic awareness and knowledge of the ecosystem that needs to surround HPC (High Performance Compute). 
- Ability to analyse and identify key knowledge in complex information from key stakeholders. 
- Experience with researchers and ability to navigate a research environment. 


## References
1. [BioNix Getting Started](https://github.com/WEHI-ResearchComputing/BioNix-GettingStarted/wiki)
2. https://github.com/PapenfussLab/bionix 
3. https://nixos.org/ 
4. https://github.com/nixos/nixpkgs
5. https://github.com/WEHI-ResearchComputing/BioNix-qc-pipe
6. https://github.com/WEHI-ResearchComputing/BioNix-Training
7. https://github.com/WEHI-ResearchComputing/BioNix-virusbreakend




