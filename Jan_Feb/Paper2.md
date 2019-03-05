## PAPER_TITLE: 
### Beyond Supervised Learning:A Computer Vision Perspective

## Authors:
Lovish Chum, Anbumani Subramaniam, C V Jawahar

Centre for Visual Information Technology IIIT-Hyderabad, Intel Bangalore, IIIT Hyderabad


## Objective:
The idea behind summarizing this paper is to provide the insight as to why modern day research work in the field of **Health Care** or even in the field of **Autonomous NAvigation** are inclining towards Unsupervised Learning.The Key issue is 'Data Scarcity' i.e.,lack of data available to train any deep learning model.

## Terminologies:
**i.)Deep Learning**:(**Internet Defn**): Is part of a broader family of machine learning methods based on learning data representations, as opposed to task-specific algorithms.

**ii.)Deep Learning**:(**Intutive meaning**):My understanding of a Deep Learning is,that it is very much evident from the name itself.**DEEP** and **LEARNING** , essentially you are trying to study some data given to you in the form of images, texts, speech, in a deep fashion, trying to exploit the deeply hidden patterns in all of these data until you get a primitive and unique representation of these data.So you are Digging Deep into the data to find some hidden pattern in them.
 
**iii.)Synthetic Data**:Typically act as a source of data augmentation, these are used along with the real data for training,and it maye cover scenarios that are not captured by real-world data.

**iv.)Domain Adaptation**:a model trained on source domain does not perform well on a target domain with different distribution. Domain adaptation (DA) is a technique which addresses this issue by reusing the knowledge gained through the source domain for the target domain.

**v.)Weakly Supervised Learning**:Weakly supervised learning is an umbrella term covering the predictive models which
are trained under incomplete, inexact or inaccurate labels

**vi.)Few Shot Learning**:Few-shot learning techniques attempt to adapt the current machine learning methods to perform well under a scenario where only a few training instances are available per class.

**vii.)Self-Supervised Learning**:In self-supervised learning, we obtain feature representation for semantic understanding tasks such as classification, detection and segmentation without any external supervision.

## Summary:
This paper basically tries to open up the space for thinking and coming up with solutions that transcend the barriers of a simple scenario of given Object-Class pairs how do you learn data (Supervised Learning).This type of learning may fail in scenarios where there is 
* Lack of Labelled Data in a particular domain.
* Unavailability of Direct Supervision:for a particular task in a given domain.

The means to tackle these problems can be categorized as follows:

* 1.) **Data-centric** techniques which solve the problem by generating a large amount of data similar to the one present in the original dataset.
* 2.) **Algorithm-centric** techniques which tweak the learning method to harness the limited data efficiently through various techniques like on-demand human intervention.
* 3.) **Hybrid** techniques which combine ideas from both the data and algorithm-centric methods.

I will try explaining you the above three methods very briefly using examples:

### Data Centric:

Data-centric techniques include data augmentation which involves tweaking the data samples with some pre-defined transformations to increase the overall size of the dataset.Again the idea here is just to increase the count of the data so that your network which you train is exposed to examples which the real-data set may not have captured. 

**Example**: In Images it may include various affine transformations, rotation, cropping, adding intensity values, adding gaussain noise

### Algorithm Centric:

Algorithm-centric techniques try to relax the need of perfectly labeled data by altering the model requirements to acquire supervision through inexact inaccurate and incomplete labels.Techniques involving on-demand human supervision have also been used to label selective instances from the dataset.
