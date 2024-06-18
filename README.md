# Vascular segmentation in the liver

Usind 3DIrcad dataset to segment vascular structures inside and around the liver with U-Net neural network using keras and tensorflow libraries in python.
1. Downland dataset using file downland_dircad.ipynb
2. Downland zip files: experiment1.zip for small U-Net arcitecture,
                       experiment2.zip for medium U-Net arcitecture,
                       experiment3.zip for large U-Net arcitecture.
3. Change the code in the file Vascular_segmentation.ipynb for work with the chosen segmented structure. (Originaly for artery segmentation with medium U-Net architecture)

# Dataset
20 CT scans of liver cancer patients, containing segmented structures such as the liver, artery (aorta and hepatic artery), vena cava, portal vein, and venous system. CT data is normalized to -1000 to 1000 Hounsfield units, with 512 x 512 x 150 px resolution coreponding to 0.7 mm x 0.7 mm x 1.6 to 4 mm) of voxelsize.

https://www.ircad.fr/research/data-sets/

Example of segmented structures in the dataset (red - arteries, green - venous system, blue - portal vein):
![image](https://github.com/romova/Liver-vascular-segmentation/assets/93135199/f2efd97c-1710-47eb-85f5-1b4ae4b86c39)

Results of models acording to dice coefficient (blue - True positive, purple - False positive, yellow - places where model prediction is better than original segmentation):
![image](https://github.com/romova/Liver-vascular-segmentation/assets/93135199/427af1a7-8211-4162-b03a-73fd3536d710)
