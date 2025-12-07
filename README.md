# Home-assignment-functional-mapping-of-hippocampal-regions
This repository contains a visualization of the functional mapping of hippocampal regions on MRI scans.

#the content of the first markdown cell
import os
os.getcwdb()
import nibabel as nib
import matplotlib.pyplot as plt
import glob
import numpy as np

from nilearn import image, plotting
from nilearn.image import smooth_img


#Contents:
#'home-assigment-functional-mapping-of-hippocampal-regions' is a notebook containing the functional and anatomical data of hippocampal brain regions that show functional activity when a person is participating in an uniformity test. The funtional and anatomical MRI data files are located automatically and smoothened to improve the interpretation. The data is visualized with a functional scan over an anatomical scan to provide information about functional voxel activation during the uniformity test in hippocampal regions. Additionally the notebook contains a code for a histogram of voxel activation values.

#Data
This project uses two MRI files from https://neurosynth.org/analyses/terms/hippocampus/:

anatomical.nii.gz
    This is a structural T1-weighted MRI used as the anatomical background image.

hippocampus_uniformity-test_z_FDR_0.01.nii.gz
    This is the functional z-statistic map representing hippocampal uniformity measures.


#Packages that are used for this notebook
    nibabel
    nilearn
    numpy
    matplotlib
    golb,os