## PAPER_TITLE: 
### Machine Learning Methods for Histopathological Image Analysis (Computational and Structural Biotechnology Journal 16 (2018) 34–42)

## Authors:
Daisuke Komura,Shumpei Ishikawa

Department of Genomic Pathology, Medical Research Institute, Tokyo Medical and Dental University, Tokyo, Japan


## Objective:
This Paper gave an idea about how Machine Learning Algorithms help in automation of Histopathological Images(Image modality for study of tissue) and thus helping the pathologists come up withe results quicker with improved accuracy

## Basic Definitions:
**i.)Whole Slide Images(WSI)**: Digital Image representation of the images of Tissues, on which one or several of the ML algorithms can be applied

**ii.)Pathology**:Specimen containing tissues of human body to be analyzed

**iii.)Histopathology**:Study of tissues of human body for analysing the manifestation of a disease

**iv.)Cancer**:A new growth of cell which has the ability to invade surrounding tissues and spread to organs .

**v.)Tumour**: Not necessarily a cancer, it refers to a mass.When the cells in the tumor are normal, it is **benign**. When the cells are abnormal and can grow uncontrollably, they are **cancerous cells**, and the tumor is **malignant**

## Summary:

The whole idea of the paper is to give light how several machine learning algorithms can help in analysis of Histopathology images of tissue, the steps that must be taken when carrying out the algorithm, preprocessing that is necessary before applying the algorithm and how different are these images from a common Digital Image that we come across.

### Where does the Role of ML come handy in histopathology image analysis??
* With Digitization of Medical Information and advances in **genome analysis**, large amount of digital info. is available.
* Analysing relationship between these data, new clinicopathological relationships can be derived 
* Ex:Relation between Morphological characteristics,semantic mutation of cancer can be found. Ultimately all of these follow some patterns and that is what the idea of deep learning is, trying to understand the underneath pattern hidden in these process by digging deep.
* But data being enormous, it is not practical for pathologists and researchers to analyse the relation manually.Hence **ML** methods
 
### Scope of Machine Learning Algorithms on Histopathology:
* WSI as a whole are analysed in patches, and each of these patches can be sent to one of the classical ML algorithms of classifying it as Cancerous vs Non Cancerous or Benign vs Malignant Tumour.The same idea can be extended to Deep Learning Architechture as well
* **Deep Learning** especially using **CNN** has the advantage that features and classifiers are simultaneously optimized, and features learned in DL often outperforms other features in Histopathology image analysis
* Unsupervised algorithms like **K-means, PCA, Auto-encoders** also aid in the task of Histopathology Image analysis
* **Content Based Image Retrieval**: The idea is to retrieve similar images to a query image.It doesnot need label information.Here not only accuracy but also high speed for search and lock is needed.so here we go for methods like **PCA**, **fast approximation**, **Nearest Neighbour search** like **Kd-Tree,Hashing** becomes important

### Problems Seen in Histopathological Images:
* **Large Image Size** :
  * WSI's typically have 1000X1000 images.Deep Learning Methods need smaller sized images.If Resizing is done as done for ordinary images would lead to loss of information at cellular level,resulting in marked decrease of identification accuracy 
  * **Solution**: Analysis is carried out by considering patches of the WSI, with or without overlap
* **Method of Integrating result of algorithm on each patch**: 
   * Even if individual patches are correctly classified, the WSI containing 100's - 1000's of patches, may generate False positives.
   * **Solution** :Regional averaging of each decision, such that regions is classified as ROI, only when ROI extends over multiple patches.Again chances of missing small ROI's such as isolated tumours may occur
* **Availability of Labelled Data**: 
   *Even though there is availability of datasets, the **WSI's** in these repositories contain label at the case-level, and to use them as training data, some pre-processing or specialized M.L algorithm is needed.
* Solution to the above said problem has a number of approaches
   *Efficient Increase of Labeld Data: One basic way is to reduce the workin time of pathologists to specify ROI's in WSI.Eventhough there are GUI's that help in annotation, localizing the ROI's accurately is not always easy.The go to solution for this is **ACTIVE LEARNING** 
### Brief Idea about Active Learning:
Active Learning is a method used in supervised Learning, and it automatically chooses the most valuable unlabelled sample, the one aht is expected to improve the identification performance of classifiers when labelled correctly and used as Training Data

## What Next!!??? 
As a continuation of this  I will be summarizing about the idea of how Unsupervised Techniques can actually help in some of these tasks and also discuss about an idea of thinking beyond supervised learning on a Computer Vision Perspecive.All this coming up in Paper2.!!!
