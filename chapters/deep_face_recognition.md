

# Face Recognition
There are three modules needed for FR system, as shown in Fig. 3. First, a face detector is used to localize faces in images or videos. Second, with the facial landmark detector, the faces are aligned to normalized canonical coordinates. Third, the FR module is implemented with these aligned face images.

FR can be categorized as face verification and face identification. In either scenario, a set of known subjects is initially enrolled in the system (the gallery), and during testing, a new subject (the probe) is presented. After the deep networks are trained on massive data with the supervision of an appropriate loss function, each of the test images is passed through the networks to obtain a deep feature representation. Using cosine distance or L2 distance, face verification computes one-to-one similarity between the gallery and probe to determine whether the two images are of the same subject, whereas face identification computes one-to-many similarity to determine the specific identity of a probe face.

deep FR always follow those of deep object classification and are modified according to unique characteristics of FR
## Survey paper
[Wang, Mei, and Weihong Deng. "Deep face recognition: A survey." Neurocomputing 429 (2021): 215-244.](https://reader.elsevier.com/reader/sd/pii/S0925231220316945?token=41B5F7C7660003AD3BB2D9B265E7DCDBC8004913684C49FD6A4EDBB9B1CB85BEB95E776C07F595BFC49C1D9F89E28B17&originRegion=us-east-1&originCreation=20220204075243), #cite: 600
## Landmark papers
* DeepFace: [Taigman, Yaniv, et al. "Deepface: Closing the gap to human-level performance in face verification." Proceedings of the IEEE conference on computer vision and pattern recognition. 2014.](https://openaccess.thecvf.com/content_cvpr_2014/papers/Taigman_DeepFace_Closing_the_2014_CVPR_paper.pdf), #cite: 6239
* DeepID
    * 
* FaceNet
* VGGFace
    * VGGFace2
* SENet

## Datasets
* LFW benchmark
* JB-A/B/C
* Megaface
* MS-Celeb-1 M

## Loss
The softmax loss is commonly used as the supervision signal in object recognition, and it encourages the separability of features. However, the softmax loss is not sufficiently effective for FR because intra-variations could be larger than inter-differences and more discriminative features are required when recognizing different people. Many works focus on creating novel loss functions to make features not only more separable but also discriminative

* Euclidean-distance-based loss
* angular/cosine-margin-based loss
* softmax loss

# Applications
* face verification
* face identification
* face detection

* anti-attack, cross-pose FR, and cross-age FR