# DECODE_for_Robust_Image_Classification
* Due to the demand for a large number of labeled samples,how to collect a sufficient training set seems to be a critical issue for deep CNN model training.</br>
* One may observe that the current training strategies simply assume that there is a relatively clean dataset available for model training, which is collected by, for example, expert labeling.
This assumption holds for many elaborately constructed benchmarks,like ImageNet. 
However, in practice, collecting such a large labeled training set is expensive and burdensome.</br>
* For example, collecting labeled samples from Internet, e.g., retrieving images from image search engine like Google using target keyword, turns out to be a convenient and economical way, which has drawn attention from some works.
It can provide nearly labor-free labeled images with potentially unlimited size.</br>
* Unfortunately, Web
images are very noisy in practice. For example, we use a keyword “dog” to retrieve images from
Google image search engine. In the top-ranked images,
there are several non-dog images, like cat images. When
there are label noise, the performance of deep CNN models
may drop dramatically.
</br>
</br>

![high_level_architecture](https://github.com/Khushi-Mineeyar/DECODE_for_Robust_Image_Classification/assets/87527377/ad2b6242-96cc-4f27-a7ec-96e054ee4fcb)

* It should be pointed out that the existing training strategies assume that there is a clean dataset for model learning.
* However, in real-world applications, it is burdensome and expensive to collect sufficient clean training samples.
* On the other hand, collecting noisy labeled samples is very economical and practical.
* Unfortunately, the accuracy of current deep models may drop dramatically even with 5%–10% label noise.
* Therefore, enabling label noise resistant classification has become a crucial issue in the data driven deep learning approaches.
* In particular, based on the distribution of mislabeled data, we adopt a confidence evaluation module that is able to determine the confidence that a sample is mislabeled.
*  With the confidence, we further use a weighting strategy to assign different weights to different samples so that the model pays less attention
to low confidence data, which is more likely to be noise. In this way, the deep model is more robust to label noise. 
