# XAI606
Applications and Practice in Neural Networks Project I

I. Project Title: Multi-Label Recognition with Limited Annotations

II. Project introduction
  - Objective: Multi-Label Recognition is essentially when the objective is to detect multiple objects in an image. However, in this scenario, not all of the labels are provided, thus making this a weakly-supervised problem. For each instance you will only have a partial set of labels, but must predict and detect all of the labels.
  - Motivation: Many datasets are only labeled for the multi-class classification problem, but in the real world are converted and used for the multi-label classification problem. Thus there is a need for models that have both supervised and unsupervised characteristics. Note that this is not a semi-supervised learning problem, as in SSL you divide the dataset into labeled and unlabeled instances, whereas in this problem, each instance contains both supervised and unsupervised characteristics.

III. Dataset Description
  - We will use the PASCAL-VOC dataset, where you can download the images here:

  - Note that while PASCAL-VOC contains a full set of annotations for the training, validation, and test, those are NOT the annotations we will be using as we are simulating a partial label problem. Instead the partial annotations can be found here:
