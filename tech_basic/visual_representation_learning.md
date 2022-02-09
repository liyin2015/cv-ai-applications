# Visual representation learning
* Large-scale supervised (images only). Can see benchmarking from [1].
* Large-scale text and image pairs -> visual representation learning in the wild! This enables (1) open vocabulary: from close-set to open-set visual recognition (2) domain adaption: from one dataset to many downstream datasets and tasks (3)transfer learning includes zero-shot and few-shot learning. 

## Supervised Images Only
The majority pretraining focus on using classification cudated datasets.
* pretrained on [ImageNet1k or ImageNet21k](https://www.image-net.org/). 
* [OpenImages](https://storage.googleapis.com/openimages/web/index.html)
* [JFT-300M](https://paperswithcode.com/dataset/jft-300m)
* Instagram hashtag datasets.

An open question: how to pretrain a model that can perform well in tasks that not only requires semantic understanding but also geo-localization, such as object/instance detection and semantic/instance segmentation?
### Applications
* Image to image retrieval
* Backbone for downstream tasks

## SSL Images only
### Landmark papers
* 
## Image and text pairs
See [Visual language model](vision_language_models.md) 
## Resources
1. [Kolesnikov, Alexander, et al. "Large scale learning of general visual representations for transfer." (2019).](https://onikle.com/articles/13442)