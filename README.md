# NNDSP

This file contains a summary of all NNDSP files/directories contents.

## anal
The anal directory contains all the notebooks and analysis material that you could ever dream of. Just kidding. Here's what's really in this folder:

1. analysis_notebooks: Folder with jupyter notebooks for study and data analysis
2. baracus_files: This directory has two subdirectories. 'analysis_notebooks/' contains notebooks 
to run baracus and  'other_files/' contains the Baracus singularity image and the swarm output. 
3. freesurfer_files: This folder contains two directories. 'analysis_notebooks/' contains the 
notebook to run freesurfer and 'other_files/' contains different singularity images
(some for freesurfer version 6, some for version 5.3). This folder also contains swarm outputs 
when freesurfer runs a swarm command on HPC. 
4. heudiconv_files: Here's the breakdown of this directory:
	- conda_env.yml: The conda environment used to run the jupyter notebooks
	- heudiconv_generic_swarm2017_06_29.cmd, heudiconv_generic_swarm2017_07_14.cmd, heudiconv_swarm2017_06_29.cmd, heudiconv_swarm2017_07_14.cmd: these are all files generated while running the jupyter notebook that hold command line commands to run heudiconv conversion.
	- heudiconv_with_sequence_name.img: the heudiconv singularity image
	- heuristics: this is a directory containing heuristics for converting DICOMS into BIDS.  
6. NCR: This folder contains the original NNDSP dataset, still in tar.gz format.
7. NKI: This folder contains all the NKI data that I downloaded. It is already in BIDS format.

## derivatives
Derivatives contains other directories with derivatives from NKI BIDS, NNDSP BIDS and some HCP BIDS
## nino
This directory contains the following:

1. HCP_ages.csv: A csv with the real ages of HCP subjects. This file is restricted access, I believe. 
As stated by the name of this directory, only I can access it.
