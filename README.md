# COVID-19 X-Ray Detection

**Abstract:**

Detection of Covid-19 using chest X-Rays are done by professionals in the medical field. It is not easily identifiable by the naked eye. It is entirely possible that sometimes even doctors get the diagnosis wrong. By using machine learning, a Covid-19 detection model will provide faster and more accurate results. A CNN model is used due to its image processing capability. It is used to compare multiple different X-Rays of patients to identify those who are infected. From the metadata, we obtain only the COVID-19 infected X-Rays, which were taken from the Postero Anterior (PA) view. From Kaggle, we take the non-infected images. We take 50-50 split and sort it into another dataset. We split this dataset into Training, Testing and Validation datasets. We preprocess the images to decrease runtime and increase response, and to standardize the data. A Feed Forward Neural Network is formed using DensetNet121, Flatten and Dropout. It uses Binary Cross-Entropy loss to give us a binary response, and transfer learning for increased efficiency. The model is generated using the Training and Testing datasets, and is run against the Validation dataset for 8 epochs (for this model). The model with the best response is from here on out used to confirm or deny infection.

**Software Design:**

Infected and non-infected Chest X-Rays forms the database used for the CNN model, made from python, to identify and detect the virus. The image to be detected is preprocessed to ensure similar reading and run through the model, which gives the result of whether the image is of an infected person or not.

**Model Loss over 8 epochs:**

![image](https://user-images.githubusercontent.com/41417732/99144057-ad4f5f80-2688-11eb-9551-90d308c78fd8.png)

**Model accuracy over 8 epochs:**

![image](https://user-images.githubusercontent.com/41417732/99144086-d112a580-2688-11eb-8863-dda2d5fc72b8.png)
