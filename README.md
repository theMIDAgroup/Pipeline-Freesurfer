# Pipeline-Freesurfer
MRI Segmentation Pipeline with Freesurfer and Optional Processing with Petsurfer

Requirements: Python3, numpy, pandas, mahotas, nibabel, Freesurfer, FSL, ANTs, Nipype, Dcm2niix

* 01: Convert T1 MRI from DICOM to Nifti and then to mgz format
* 02: Execute Freesurfer's ReconAll for structural analysis
* 03: Transform Aparc (cortical VOIs in both hemispheres) and Aseg (sub-cortical VOIs) outputs to a tabular format
* 04: Perform additional GTM segmentation on the T1 MRI
* 05: Convert FDG PET from DICOM to Nifti format
* 06: Spatially normalize FDG PET and GTMSeg to MNI coordinates
* 07: Normalize intensities of the FDG PET
* 08: Conduct Regional Analysis of FDG PET, resulting in the mean FDG uptake in all segmented regions
