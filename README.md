" Privacy_Protection_MaskRCNN_InceptionV2" 
e.
Mask-RCNN was initially introduced in Nov 2017 by Facebook’s AI Research team using Python and Caffe2.This is an implementation of Mask R-CNN on Python 3.Privacy is protected by detecting sensitive objects and segmenting those from video.The model can generate bounding boxes and segmentation masks of each instance in the image.It's based on InceptionV2 backbon.The Mask-RCNN algorithm produces the predicted detection outputs as the bounding boxes. Each bounding box is associated with a confidence score. All the boxes below the confidence threshold parameter are ignored for further processing.The object mask output from the network is a greyscale image. One could use it directly for alpha blending purposes, if needed.we use the maskThreshold parameter to threshold the grey mask image.We can reduce its value would result in a larger mask. Sometimes this helps include the parts missed near the boundaries, but at the same time, it might also include the background pixels at the more pointy boundary regions and more noises.One thing to remember,lowering the threshold value you may also can gain mask of object at a distance which is hardly noticed by people too.
