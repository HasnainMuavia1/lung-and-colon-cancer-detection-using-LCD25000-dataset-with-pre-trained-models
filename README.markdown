**Lung and Colon Cancer Detection with Deep Learning using LCD25000
Dataset**

This document explores the application of deep learning for lung and
colon cancer detection using the LCD25000 dataset.

**Dataset:**

-   Name: LCD25000

-   Size: 25000 histopathological images

-   Distribution:

    -   5 Classes (5000 images each)

        -   Lung Cancer:

            -   lung_aca (Lung Adenocarcinoma)

            -   lung_n (Lung Benign Tissue)

            -   lung_scc (Lung Squamous Cell Carcinoma)

        -   Colon Cancer:

            -   colon_n (Colon Benign Tissue)

            -   colon_aca (Colon Adenocarcinoma)
            -   
**Requirements:**
- tensorflow
- python 3.x
- numpy
- pandas
- keras
- sklearn
- 
**Models:**

-   DenseNet121

-   VGG-16

-   VGG-19

**Modifications:**

-   DenseNet121:

    -   Added Flatten layer

    -   Added Dense layer with 128 neurons

-   VGG-16:

    -   Retrained Block 5 for fine-tuning

    -   Added Flatten layer

    -   Added Dense layer with 128 neurons

-   VGG-19:

    -   Retrained Block 5 for fine-tuning

    -   Added Flatten layer (no additional Dense layer)

**Results Best Model:**

The best performing model was VGG-16 with a test accuracy of 99.24%.

**Discussion:**

-   This study demonstrates the effectiveness of deep learning models
    for classifying lung and colon cancer from histopathological images.

-   VGG-16 achieved the highest accuracy, suggesting its potential for
    this specific task.

-   Fine-tuning pre-trained models like VGG-16 with additional layers
    can improve performance.

-   DenseNet121 with additional layers also achieved good results,
    highlighting the potential of alternative architectures.

**Train, Test, Validation:**

1.  **Train 80%**

2.  **The rest is distributed 50 by 20 to validation and test**

**Model Performance on LCD25000 Dataset (Including Training Results)**

| Model     | Train Loss | Train Accuracy | Validation Loss | Validation Accuracy | Test Loss | Test Accuracy |
| ---------- | --------: | --------------: | --------------: | --------: | --------: | --------: |
| DenseNet121 | 0.0096     | 0.9979           | 0.0228           | 0.9940     | 0.0290     | 0.9904     |
| VGG-16     | 0.0089     | 0.9975           | 0.0205           | 0.9900     | 0.0254     | 0.9924     |
| VGG-19     | 0.0110     | 0.9965           | 0.0270           | 0.9896     | 0.0283     | 0.9892     |


**DenseNet121:**

**Accuracy:**

![A graph with a line and a line Description automatically generated
with medium
confidence](vertopal_9343de9989524c4e8b53a44758a9c201/media/image1.png)

**Loss:**

![A graph with red and blue lines Description automatically
generated](vertopal_9343de9989524c4e8b53a44758a9c201/media/image2.png)

**Confusion matrics:**

![A diagram of a number of cells Description automatically generated
with medium
confidence](vertopal_9343de9989524c4e8b53a44758a9c201/media/image3.png)
**VGG-16**

**Accuracy:**

![A graph with a line and a red line Description automatically
generated](vertopal_9343de9989524c4e8b53a44758a9c201/media/image4.png)

**Loss:**

![A graph of a line Description automatically generated with medium
confidence](vertopal_9343de9989524c4e8b53a44758a9c201/media/image5.png)

**confusion matrix:**

![A diagram of a number of cells Description automatically generated
with medium
confidence](vertopal_9343de9989524c4e8b53a44758a9c201/media/image6.png)
**VGG-19**

**Accuracy:**

![A graph with a red line and blue line Description automatically
generated](vertopal_9343de9989524c4e8b53a44758a9c201/media/image7.png)

**Loss:**

![A graph with a red line and blue line Description automatically
generated](vertopal_9343de9989524c4e8b53a44758a9c201/media/image8.png)

**Confusion matrix:**

![A diagram of a diagram Description automatically generated with medium
confidence](vertopal_9343de9989524c4e8b53a44758a9c201/media/image9.png)

## Authors

- [@HasnainMuavia](https://github.com/HasnainMuavia1)


