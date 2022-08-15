# BioNix Student Internship Project


This project would suit a research software engineering candidate who was interested in reproducibility, wants to gain experience with executing bioinformatics workflows efficiently, and enjoys streamlining complex processes.

Bioinformatics as a discipline frequently uses many individual software tools, connected in potentially complicated ways, to perform typical analysis. As an example, standard Single Nucleotide Variant (SNV) calling in cancer involves alignment of the sequencing reads to a reference genome, sorting and indexing, variant calling, and subsequent annotation against various databases. Each of these stages comprises of one or more software tools with different input requirements. 

As a result, reproducibility is difficult to achieve due to the large number of components and the complicated dependency structure inherent in both building the software tools and execution of the workflow. A recently proposed solution to the problem, BioNix[1], leverages the Nix[2] functional package management system to both manage the software and execute the workflow. This has allowed an unprecedented level of reproducibility in the field. 

The candidate will be responsible for expressing various bioinformatics processing pipelines in the BioNix workflow framework. The goal is to write a variety of standard processing pipelines within the framework, making typical analysis both easily accessible and highly reproducible to many bioinformatics researchers. 

This will include: 
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

Expected outcomes:
- Wrapping at least 2 whole bioinformatics workflows with all underlying bioinformatics software using nixpkgs with full testing of each stage and as a whole on two different compute platforms.

Possible Mentors:
- Justin Bedo
- Matthew Wakefield
- Rowland Mosbergen

Expected Size of Project:
- 350 hours

Difficulty rating:
- Medium
