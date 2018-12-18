# Deep spectral-based shape features for Alzheimer’s Disease classification

This repository contains information about the paper entitled "Deep spectral-based shape features for Alzheimer’s Disease classification"
# Manuscript abstract
Alzheimer’s disease (AD) and mild cognitive impairment (MCI) are the most prevalent neurodegenerative brain diseases in elderly population. Recent studies on medical imaging and biological data have shown morphological alterations of subcortical structures in patients with these pathologies. In this work, we take advantage of these structural deformations for classification purposes. First, triangulated surface meshes are extracted from segmented hippocampus structures in MRI and point-to-point correspondences are established among population of surfaces using a spectral matching method. Then, a deep learning variational auto-encoder is applied on the vertex coordinates of the mesh models to learn the low dimensional feature representation. A multi-layer perceptrons using softmax activation is trained simultaneously to classify Alzheimer’s patients from normal subjects. Experiments on ADNI dataset demonstrate the potential of the proposed method in classification of normal individuals from early MCI (EMCI), late MCI (LMCI), and AD subjects with classification rates outperforming standard SVM based approach.

# Dataset
The original data comes from the popular brain imaging dataset in Alzheimer’s disease, namely the Alzheimer’s Disease Neuroimaging Initiative (ADNI: adni.loni.usc.edu). For this study, a subset of latest 1.5 T MR images is used including 150 normal controls (NC), 90 AD patients, 160 early MCI (EMCI), and 160 individuals with late MCI (LMCI). Left (label number 17) and right (label number 53)hippocampi were segmented using FSL-FIRST automatic segmentation software package. Some subjects were removed because of the failure in the preprocessing steps. Therefore, in total, 142 normal controls (NC), 83 AD patients, 154 early MCI (EMCI), and 150 individuals with late MCI (LMCI) were included in our analysis.

The folder data includes 4 sub-folders (NC, AD, EMCI, LMCI). Each folder contains two sub-directories (17 and 53). All the spectral meshes in vtk format are saved here.

# Citation
If you find our mesh dataset useful for your research, please first cite our paper:

```@inproceedings{shakeri2016subcortical,
    Author = {Shakeri, Mahsa and Tsogkas, Stavros and Ferrante, Enzo and Lippe, Sarah and Kadoury, Samuel and Paragios, Nikos and Kokkinos, Iasonas},
    Title = {Sub-cortical Brain Structure Segmentation Using F-CNNs},
    Booktitle = {International Symposium on Biomedical Imaging ({ISBI})},
    Year = {2016}
}```

ur mes
