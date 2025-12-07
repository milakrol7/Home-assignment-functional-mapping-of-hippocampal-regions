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
#This notebook contains the functional and anatomical data of hippocampal brain regions that show functional activity when a person is participating in an association test. The first image shows a 4D brain scan that can be used to navigate through the brain to identify voxels, and thus brain regions, that are associated with association activities. The second image shows a histogram with the functional activity per voxel, indicating which hippocampal brain areas show the most activation.
