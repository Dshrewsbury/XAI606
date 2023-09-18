# I. XAI606: Multi-Label Recognition with Limited Annotations
Applications and Practice in Neural Networks Project I

## II. Project Introduction
  - Objective: Multi-Label Recognition is essentially when the objective is to detect multiple objects in an image. However, in this scenario, not all of the labels are provided, thus making this a weakly-supervised problem. For each instance you will only have a partial set of labels, but must predict and detect all of the labels.
  - Motivation: Many datasets are only labeled for the multi-class classification problem, but in the real world are converted and used for the multi-label classification problem. Thus there is a need for models that have both supervised and unsupervised characteristics. Note that this is not a semi-supervised learning problem, as in SSL you divide the dataset into labeled and unlabeled instances, whereas in this problem, each instance contains both supervised and unsupervised characteristics.

## III. Dataset Description
  - We will use the PASCAL-VOC dataset, where you can download the images here: http://host.robots.ox.ac.uk/pascal/VOC/voc2007/

  - Note that while PASCAL-VOC contains a full set of annotations for the training, validation, and test, those are NOT the annotations we will be using as we are simulating a partial label problem.
  - Instead the partial annotations can be found here: https://drive.google.com/drive/folders/1h1ML-BqwZIQBM9kl_U7IMZFJwzosQ8BP?usp=drive_link

    processed_trainval_images_2007.npy contains the image names for each image in pascal vocs training and validation set. The rows in this file correspond to processed_trainval_labels_2007.npy and partial_random_50_trainval_labels.npy, which are the annotations for the training and validation set. The annotations in processed_trainval_labels_2007 should only be used for validation and development purposes, but all training should be done with the labels in partial_random_50_trainval_labels.npy. The labels in that file contain the values: 1,0, -1. 1 for positive labels, 0 for negative labels, and -1 to indicate that the label is missing. processed_test_images_2007.npy contain a list of the images in the test set, but do not contain the labels.

    Note: all of the images_2007.npy files correspond to the images found in the VOCdevkit/VOC2007/JPEGImages folder.
