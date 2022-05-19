# EllipDet
## Ellipse detection datasets and algorithms
Public datasets for ellipse detection usually have different formats, such as the rotation angle, some use radians, while others use angles. We sort out seven publicly most used datasets for easier use. Besides, we further build an industrial dataset by a BFS-PGE-23S3M-C Point Grey camera. 

## Two synthetic datasets:
1. Occluded dataset. It contains 600 images, and each image has {4, 8, 12, 16, 20, 24} occluded ellipses. The original format is .mat which must be processed by MATLAB. We transform it to .jpg which is more general for use.
2. Overlapping dataset. It also contains 600 images, and each image has {4, 8, 12, 16, 20, 24} ellipses. We also transform the .mat format to the .jpg format.

## Five real-world datasets:
1. Dataset Prasad. The original dataset contains 400 images from 48 categories in the Caltech256 dataset, however, there are only 198 images remained. To boost the development of ellipse detection algorithms, we complete the missing images according to the file provided by Prof. Prasad, hence there are 400 images. All ground truth are labeled by ourselves manually and precisely.
3. Dataset #1. A multi-class dataset contains 400 images from the MIRFlickr and LabelMe repositories.
4. Dataset #2. This dataset containing 629 images is collected from several videos.
5. Dataset PCB. A printed circuit board dataset contains 100 images.
6. Dataset Calibration. This dataset is used for camera calibration, despite only containing 40 images, there are at least 70 ellipses in each image. The original image is .pgm format, which usually cannot be opened. We transform the .pgm to .jpg for easier use.

## Additional industrial dataset:
We further provide a dataset for industrial measurement purpose. There are in total of 77 images that either come from different industrial components or come from different perspectives of the same component. 

All datasets contain original images in the 'xx/images' format and the GT in the 'xx/gt' format. We also unify the GT format as 'gt_imageName.txt', hoping to be easier used for more people.

# Acknowledgements
Since most datasets are provided by previous authors, we give great thanks to Dr. Dilip K. Prasad, Dr. Michele Fornaciari, Dr. Qi Jia, Dr. Changsheng Lu, Dr. Viorica Pătrăucean, and Dr. Alex Yong-Sang Chia. Thank you very much for the efforts and sharing such useful datasets. 
