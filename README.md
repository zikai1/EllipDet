# EllipDet
Ellipse detection datasets and algorithms
Public datasets for ellipse detection usually have different formats, such as the rotation angle, some use radians, while some use angles. We sort out seven publicly most used datasets for easy use. Besides, we further build an industrial dataset by a BFS-PGE-23S3M-C Point Grey camera. 

Two synthetic datasets:
1. Occluded dataset. It contains 600 images, and each image has {4, 8, 12, 16, 20, 24} occluded ellipses. The original format is .mat which must be processed by MATLAB. We transform it to .jpg which is more easier for use.
2. Overlapping dataset. It also contains 600 images, and each image has {4, 8, 12, 16, 20, 24} ellipses. We also transform the .mat format to .jpg format.

Five real-world datasets:
1. Dataset Prasad. The original dataset contains 400 images from 48 categories in the Caltech256 dataset, however, there are only 198 images remaining. To boost the development of ellipse detection algorithms, we complete the lost images according to the file provided by Prasad, and label the ground truthes by ourselves manually and precisely.
2. Dataset #1. A multi-class dataset contains 400 images from the MIRFlickr and LabelMe repositories.
3. Dataset #2. This dataset containing 629 images is collected from several videos.
4. Dataset PCB. A printed circuit board dataset contains 100 images.
5. Dataset Calibration. This dataset is used for camera calibration, although only containing 40 images, there are at least 70 ellipses in each image. The original image is .pgm format, which usually cannot be opened. We transform the .pgm to .jpg for easy use.

Additional industrial dataset:
We further provide a dataset for industrial measurement. There are in total of 77 images that either come from different industrial components or come from different perspectives of the same component. 
