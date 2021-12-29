# ImageSegmentationWithFCN

The above repository corresponds to an assignment for the course Advanced Computer Vision taken under Prof. Ram Nevatia at USC in fall 2021

Image Segmentation on the KITTI dataset has been performed here using two architectures - FCN16 and FCN32 (https://arxiv.org/abs/1411.4038) - however the backbone used was ResNet18 - using deeper ResNet's should be a straightforward change in the code files.

ResNet18's were appropriately modified to make the output the same dimensions as the input image and the network was made fully convolutional - the way this modification was done can be found in the Report PDF document.

It should be noted that the input images haven't been cropped - the train/val/test sets were batched such that cropping wasn't needed for the dataloader, however, to use in a more general sense, the input image and the ground truth image should be appropriately cropped - online/offline augmentations also weren't performed and should be applied appropriately if one wants to improve the results.

NOTE - the link to the colab files have been provided here, the code runs on a single GPU. Result folders with relevant visualizations and comparions and a report PDF have also been included in the folder.
