# Multi-Label-Ocular-Disease-Classification_Transfer-learning

## Dataset
Ocular Disease dataset (ODIR) is a structured ophthalmic database of 1802 patients with images and classification of pathology.

This dataset is meant to represent ‘‘real-life’’ set of patient information collected by Shanggong Medical Technology Co., Ltd. from different hospitals/medical centers in China. In these institutions, fundus images are captured by various cameras in the market, such as Canon, Zeiss and Kowa, resulting into varied image resolutions.
Annotations were labeled by trained human readers with quality control management. They classify patient into six labels including:
- Normal (N),
- Diabetes (D),
- Glaucoma (G),
- Cataract (C),
- Age related Macular Degeneration (A),
- Pathological Myopia (M),

![download](https://user-images.githubusercontent.com/78934727/157920405-6d46d414-7c52-471b-93dd-5d7105a174e5.png)


## Prerequisites

-Google Colab

-Keras

-some basic packages

## Model
Transfer learning is a machine learning method where a model developed for a task is reused as the starting point for a model on a second task.

It is a popular approach in deep learning where pre-trained models are used as the starting point on computer vision and natural language processing tasks given the vast compute and time resources required to develop neural network models on these problems and from the huge jumps in skill that they provide on related problems.

##### Pre-trained Model Approach
- **Select Source Model** A pre-trained source model is chosen from available models. Many research institutions release models on large and challenging datasets that may be included in the pool of candidate models from which to choose from.
- **Reuse Model** The model pre-trained model can then be used as the starting point for a model on the second task of interest. This may involve using all or parts of the model, depending on the modeling technique used.
- **Tune Model** Optionally, the model may need to be adapted or refined on the input-output pair data available for the task of interest.

In my case, I reuse and adapt the famous convolutional neural di netework VGG16.

## Results

The results of the multi-label classification are:

- TRAINING ACCURACY: 84,38%

- VALIDATION ACCURACY: 78,16%

![acc](https://user-images.githubusercontent.com/78934727/157920309-b6b24684-d276-432e-baac-2d61d61da857.png)
![loss](https://user-images.githubusercontent.com/78934727/157920334-ecfb4e38-7ff2-4cac-aa80-acacac60dc27.png)
