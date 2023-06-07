# Neural Networks and Deep Learning Project
Predict and classify gender and age groups of people based on faces captured in images

This project is done for the Singapore NTU SCSE module CE4042 Neural Networks and Deep Learning. The dataset used in this project is from the [Adience Dataset](https://talhassner.github.io/home/projects/Adience/Adience-data.html#agegender). This project is also based on a published work done by G. Levi and T. Hassner.[^1]

Aim of the project: With the Adience dataset, improve the classification of gender and age from the published work of G. Levi and T. Hassner.[^1]

How this project was conducted:
- Data exploration, alanysis and preprocessing was done on the Adience dataset to see the distribution of classes for age groups and gender.
- We explore some models and boiled down to 3 models to compare performance.

The 3 models used are:
- A 5 layer convolutional neural network model created by scratch fine-tuned for best performance in this situation. (**Original Model**)
- Inception-V3 model using transfer learning (from Tensorflow hub)
- A modified Inception-V3 model from transfer learning by adding another hidden dense layer (**Modified Inception-V3**)

These 3 models are compared with the model proposed by G. Levi and T. Hassner [^1]. (**Levi-Hassner Model**)

## Results
Results for Gender Classfication:

| Model | Validation Accuracy (%) |
| --- | --- |
| Levi-Hassner Model | 86.8 |
| Original Model | 90.3 |
| Inception-V3 | 86.9 |
| Modified Inception-V3 | **92.9** |

Results for Age Group Classfication:

| Model | Validation Accuracy (%) |
| --- | --- |
| Levi-Hassner Model | 50.7 |
| Original Model | 61.6 |
| Inception-V3 | 56.0 |
| Modified Inception-V3 | **63.6** |

## Conclusion

The modified Inception-V3 model works the best. In this project, we learnt more about different types of models used in deep learning and how to do transfer learning.

[^1]: G. Levi and T. Hassner, “Age and gender classification using convolutional neural networks.” in IEEE Conf. on Computer Vision and Pattern Recognition (CVPR) workshops, 2015
