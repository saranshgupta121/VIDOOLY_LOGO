# VIDOOLY_LOGO
Logo Classification and Detection

Since the training dataset has only 810 images and 27 classes of classes.That means only 30 images per class.So the data is not sufficent to train a convolution network from scratch, hence data augmentation technique is used to increase the number of training samples.

Firstly i used OpenCv orb but the results wasn't satisfactory.So after that i used transfer learning for classsification of logos using VGG-16 network which is best for the image classification which gave a training accuracy of 98% which seems to decrease on test dataset.

For detecting the logo, template matching technique is used.

The problem with our model was due to very small region of interest(logo) on the entire image which makes our model quite hard to learn the required features.Further improvement can be done by sliding window method. For smarter region proposals, we can use  and an image-segmentation based approach allowing us to generate more finegrained region proposals without having the number of regions to test blow up too quickly.For bounding box we can use appproach of YOLO.  

