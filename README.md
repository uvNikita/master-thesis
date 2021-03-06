# Multi-label classification of a real-world image dataset

The final compiled version of the thesis is available [here](https://github.com/uvNikita/master-thesis/blob/master/Multi-label%20classification%20of%20a%20real-world%20image%20dataset.pdf). The supplementary source code is located in the separate repository: https://github.com/uvNikita/master-thesis-src

## Abstract
Deep neural networks have shown increasing performance in image classification recent years. However, most of the methods developed in research are created, trained and compared on standard, general image collections. While some of such datasets contain realistic pictures with multiple objects and interaction between them, the selection of pictures and categories is broad and designed for the training of automatic classification systems. Therefore, questions remain on how modern image classification approaches can be applied to real-world datasets. What challenges can arise in the implementation of systems based on such datasets and how can they be solved? What level of classification performance can be expected? This study looks into these questions and gives insights on building such classification systems for real-world image collections.

The Norwegian News Agency provided the author with a unique labeled dataset of one million images for the purpose of this research. The study consists of a trial and main experiment. The goal of the trial experiments was to learn necessary tools, test classification system implementation, training and testing pipelines as well as different architectural design choices. These set of experiments were performed on a subset of the original image collection with a limited number of categories. Insights from these experiments were further used to perform model training on a much broader set of manually selected categories. Two network architectures were employed and compared in the research: CaffeNet and GoogleNet.

Results from the study suggest a big potential of using pre-trained convolutional neural networks in solving the task of multi-label image classification on a real-world dataset. However, the study also highlights a number of challenges connected with developing such system in realistic environment, including:
* A unique set of categories which requires either to train a new model or to reuse a pre-trained neural network with adjustments in the architecture to solve classification problems.
* Difficulties in category tree transformation connected with the decision of which categories include, exclude and merge.
* Categories which are unsuitable for automatic training purposes including contextual, abstract and ambiguous labels.
* Contextual images which can not be classified only by visual features and require additional information.
* Issues connected with the classification of objects and people located in the background of the pictures.
* Duplicates of images in the dataset which can cause issues for both training and testing processes.

The research gives further insights on the challenges mentioned, discusses their impact and possible solutions to them. The main limitation of the study is that only
one dataset was employed in the research. Therefore, results are considered likely to be more generalizable to datasets similar to the one used in the study.
