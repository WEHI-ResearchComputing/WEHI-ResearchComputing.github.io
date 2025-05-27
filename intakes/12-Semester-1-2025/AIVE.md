
# **AIVE**

The challenge that we were trying to solve was to streamline dataflow within ParaView software. Most of the functions were performed manually on ParaView, which meant users had to manually import and export files, and individually apply filtering like creating contours to each mask. This repetitive work in filtering and adjusting parameters cause inefficiency when reproducing experiments in the software. Creating functions that tackle this problem requires knowledge of writing scripts and how to carefully integrate them into the software. 

To address the problem, we developed a user-friendly interface (UI) using the Tkinter toolbox in Python and adapted scripts from the Start Trace function in ParaView. This UI allows users to input specific parameters related to ParaView settings—such as folder paths, file prefixes, and isocontour values—which are then stored in a configuration file for automated processing within ParaView. The scripts have been successfully tested on the Milton High Performance Computing (HPC) system, enabling broader usability across WEHI. Additionally, complementary scripts (e.g., for exporting data as .stl files) were created to enhance user convenience and streamline the workflow.

Through this process, we learned how to write correct Python scripts and config files, build a smooth user interface, and test the robustness of our program in different environments including the HPC system. Additionally, we also learned soft skills like communication, collaboration, problem-solving, and critical thinking.

## Key links
- [Final presentation slides](https://docs.google.com/presentation/d/1lxnRx3ag-3WRUrhMkMs8SZ6hP-Eqi_uCd_Z6r9HGw7s/edit?slide=id.p#slide=id.p)
- [Links to the github repos that were part of this project](https://github.com/MitochondRuna/AIVE-Intro/tree/WEHI-Internship-S1-2025)
- [Links to the data needed to run the software](https://drive.google.com/drive/folders/1tYgeA7FHXffrVzm1vBYM-A8hfXKE_rT-?usp=drive_link)
- [Links to other documentation, such as technical diary and other project documentation ](https://github.com/MitochondRuna/AIVE-Intro/tree/WEHI-Internship-S1-2025/UI_for_Paraview_Processing/Final_Scripts)
