# APESS2018 Steel Girder Crack ID Data Set

The data set is used for one of the two final group projects in APESS2018.

Download link 1: https://pan.baidu.com/s/1dduIb1_mwxaMAJbMSb3GnA (size: 2.01GB)

Download link 2: https://drive.google.com/open?id=1bpB0FEB_VM2wI6-1gnK2cdLpkETETHd1 (size: 2.01GB)

## Goal of the data set
In this project, each group of participants needs to build and train a neural network, or use a popular existing network and conduct transfer learning to detect cracks in images. Except cracks, there are ruler, handwriting, and steel girder surface as another 3 classes. These images show the practical situation of manual crack inspection for long-span bridge in China.

## Contents in the data set
In the data set package, there are 4 folders:

### In folder '0_raw_images':
50 Raw crack images.

### In folder '1_image-wise_labels':
50 image-wise labels of the same resolution with the raw images.

### In folder '2_subimages_and_labels':
If you load the .mat file by MATLAB, you can readily see two variables named as 'subimage_array' and 'subimage_label'.
If you use Python, the variables in .mat file will be stored in a dictionary, and the keys are 'subimage_array' and 'subimage_label'.
subimage_array is a 4D array of size [3927, 64, 64, 3], which is stacked by the 3D subimages ([64, 64, 3]). These subimages are generated by column from each raw image.
subimage_label is a 2D numpy array in Python (or a vector in MATLAB) of size [3927, 1], which is corresponding to the subimage_array.

### In folder '3_help_codes':
You can use the python codes to generate new subimages and corresponding labels with diffrent subimage size.

## Future work
* More images could be added into the data set depending on the feedback.
* More label format would be added into the data set depending on the feedback also.
* If you want to contribute to the data set, for example, labeling raw images, or submit your labeled image at hand, please contact us.
* There is no formal paper to introduce the data set yet, so just cite the web page of the data set repository: https://github.com/dawnnao/APESS2018_Steel_Girder_Crack_ID_dataset

<br/>

Photographer: Kun Fang

© 2018 Center of Structural Monitoring and Control, Harbin Institute of Technology

