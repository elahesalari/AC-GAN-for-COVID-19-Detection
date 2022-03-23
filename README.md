# AC-GAN-for-COVID-19-Detection

I implemented the 'Data Augmentation Using Auxiliary Classifier GAN for Improved Covid-19 Detection' paper.

<b> Dataset: </b> 
<br/>
COVID, Non-COVID CT IMAGES 
<br/>
Dataset link: https://drive.google.com/drive/folders/1kVIe0HIYz_k9Jcjn27ViHPe51AG9y_fr?usp=sharings

<b> Part A: </b>In this section, you will learn a deep ConvNet to classify COVID and Non-COVID
images.
1. Divide the data into 80% for training and 20% for test of model. Note that there is
more than one image for a patient and the images of a particular patient should not be 
in both training and test data.
2. Do the necessary pre-processing on the images and resize them suitably for entering 
the network. The images in the database have different sizes.
3. Train a deep ConvNet as a classifier to distinguish between COVID and Non-COVID
CT images.
4. You can use pre-trained networks (e.g., VGG-16) to extract features, or you can train 
a new network.
5. Calculate the precision, recall, F1-score, accuracy and AUC criteria and report them.
In python, you can use SKlearn library for these metrics.
6. Plot the ROC curve.

<b> Part B: </b>The purpose of this part is to generate more images than the given dataset. You will 
train an AC-GAN to generate images while predicting their classes.
1. Do steps 1-2 of part A.
2. Train an AC-GAN to can generate COVID and Non-COVID images with labels. You 
can use any deep structure for its generator and discriminator.
3. Use the ConvNet, trained in part A, and test it with the generated (labeled) images in 
this part. Report the same metrics, calculated for them.
4. Give 20% of the original test images along with the generated images as test images 
to the trained ConvNet and report the same metrics.
5. Plot the ROC curve.

