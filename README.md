# NNDSP

This file contains a summary of all NNDSP files/directories contents.

## anal
The anal directory contains all the notebooks and analysis material that you could ever dream of. Just kidding. Here's what's really in this folder:

1. analysis_notebooks: Here's where the bulk my data analysis took place. The files contained in this folder work as follows:
	- age_distributions.ipynb: This notebook tries to mimic the age distributions of NNDSP onto NKI or HCP on NKI and NNDSP. 
	- machine_learning.ipynb: This notebook compares the complex and simple model on HCP, NNDSP and NKI.
	- phenotype_files: contains all the csv files (with sex, age, etc) of different datasets.
	- continuous_complex.ipynb: This notebook tries to continuously downsurf the complex model.
	- ninos_magic_env.yml: The conda environment used to run these notebooks.
	- stat_tests.ipynb: Jupyter notebook with statitistical functions used in machine_learning.ipynb
	- exploratory_methods.ipynb: Additional work done with his project. 
	- other_files: This file contains hcp_area.csv file that I used to submit a pull request to bids/BARACUS. The tt_split.csv contains information about multiple runs of the machine_learning.ipynb.
	- util.ipynb: This notebook has additional functions that are used in the main notebook.    
2. baracus_files: This directory has two subdirectories. They are as follows
	- analysis_notebooks: The jupyter notebook to run baracus is in directory
	- other_files: This folder contains the Baracus singularity image and the swarm output. 
3. freesurfer_files: This folder contains two directories. Here's what's in them.
	- analysis_notebooks: This contains the notebook to run freesurfer
	- other_files: This folder contains different singularity images (some for freesurfer version 6, some for version 5.3). This folder also contains swarm outputs when freesurfer runs a swarm command on HPC. 
4. heudiconv_files: Here's the breakdown of this directory:
	- conda_env.yml: The conda environment used to run the jupyter notebooks
	- heudiconv_generic_swarm2017_06_29.cmd, heudiconv_generic_swarm2017_07_14.cmd, heudiconv_swarm2017_06_29.cmd, heudiconv_swarm2017_07_14.cmd: these are all files generated while running the jupyter notebook that hold command line commands to run heudiconv conversion.
	- heudiconv_with_sequence_name.img: the heudiconv singularity image
	- heuristics: this is a directory containing heuristics for converting DICOMS into BIDS.  
5. mriqc_files: This is John's doing.
6. NCR: This folder contains the original NNDSP dataset, still in tar.gz format.
7. NKI: This folder contains all the NKI data that I downloaded. It is already in BIDS format.

## bids_2017_07_14
When running heudiconv on the NNDSP dataset, this directory was created to hold the BIDS structure result.

## bids_2017-07-14_generic
When running heudiconv on the NNDSP dataset, this directory was created to hold the DICOM files. 

## derivatives
Derivatives contains a bunch of directories with processed data. In here, you can find the following:

1. bar_hcp_subj: This directory contains the output of BARACUS on HCP data. 
2. bar_nki_subj: This directory contains the output of BARACUS on NKI data. Surprise, surprise!
3. bar_subj: Guess what? This directory contains the output of BARACUS on NNDSP data.
4. fs5.3_subj: To run BARACUS, one has to feed it the output of Freesurfer version 5.3. That is why this folder contains the freesurfer v.5.3 run on NNDSP data.
5. fs_hcp_subj: The original HCP data is in /data/HCP/HCP_900/s3/hcp. In there, they have the raw data for their 900 subjects as well as freesurfer version 5.3 outputs. I copied the files from the freesurfer output for each HCP patient that I needed to run Baracus. Thus, this folder only contains a couple of surf files and one stats file for each subject. The files I copied can be found under /data/HCP/HCP_900/s3/hcp/{subject_number}/T1w/{subject_number}
6. fs_nki_subj: I also ran freesurfer 5.3 on the NKI data and the output is in this directory.
7. fs_subj: Because I'm a dufus, I first ran Freesurfer version 6 on the NNDSP data. The out of that is contained in this directory. 
8. mriqc: It wasn't me. It was JOHN.

## nino
Not to brag, but, I have access to the real ages of the HCP subjects, which makes me pretty cool. This directory contains the following:

1. HCP_ages.csv: A csv with the real ages of HCP subjects. This file is restricted access, I believe. As stated by the name of this directory, only I can access it.

## nndsp_qc_metrics.xlsx
This file presumably contains QC metrics about the NNDSP data. I would ask John about this.

## temp_august_workshop
This directory was created for the purposes of the Reproducibility Workshop the Data Science and Sharing Team led on August 1st/2nd 2017. John put this directory into NNDSP because he wanted to double check his lesson worked (because John always screws something up).

This directory contains  

1. test.txt: This file contains header information that you can add to your ~/.ssh file in order to ssh into biowulf/helix.
2. ds000114: This direcoty contains information about subjecs, some tsv files, etc. This was used for demonstrations such as git annex during the Reproducibility Workshop. 