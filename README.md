# Mushroom Classification

This is a project intended to classify different classes of mushroom using machine learning.

## Problem Statement

The Audubon Society Field Guide to North American Mushrooms contains descriptions
of hypothetical samples corresponding to 23 species of gilled mushrooms in the
Agaricus and Lepiota Family Mushroom (1981). Each species is labelled as either
definitely edible, definitely poisonous, or maybe edible but not recommended. This last
category was merged with the toxic category. The Guide asserts unequivocally that
there is no simple rule for judging a mushroom's edibility, such as "leaflets three, leave it
be" for Poisonous Oak and Ivy.
The problem is to predict which mushroom is poisonous & which is edible.

## Approach

In response to the need for accurately identifying whether mushrooms are poisonous or edible, a sophisticated solution has been developed utilizing Support Vector Machines (SVM), a powerful machine learning technique. SVM is a supervised learning algorithm that excels at classification tasks by finding the optimal hyperplane that best separates different classes of data points.

### Dataset:
The foundation of this solution lies in a carefully curated dataset containing various features extracted from different mushroom samples. These features encompass characteristics such as cap shape, cap color, gill size, odor, and more. Each mushroom sample is labeled as either "poisonous" or "edible," forming the basis for training the SVM classifier.


[Dataset - Mushroom Classification](https://www.kaggle.com/datasets/uciml/mushroom-classification)

### Feature Engineering:
Prior to training the SVM, the dataset underwent meticulous feature engineering. This process involved selecting relevant features, handling missing data, and potentially performing transformations to improve the discriminatory power of the features. Feature scaling might have been applied to ensure that all features contribute equally to the model's performance.

### Model Training:
The heart of the solution is the SVM classifier. The classifier was trained using the labeled dataset, aiming to learn the optimal decision boundary that effectively separates the two classes: poisonous and edible mushrooms. SVM's ability to handle non-linear boundaries, thanks to the kernel trick, makes it particularly well-suited for this task.

### Hyperparameter Tuning:
To achieve the best performance, an essential step is hyperparameter tuning. Parameters like the type of kernel (linear, polynomial, radial basis function, etc.), kernel parameters, and regularization parameters are optimized to maximize the classifier's predictive accuracy while avoiding overfitting.


### Model Evaluation:
The effectiveness of the SVM classifier was assessed through rigorous evaluation using metrics such as accuracy, precision, recall, F1-score, and confusion matrices. Cross-validation techniques might have been employed to estimate the model's performance on unseen data and guard against over-optimistic results.

### Results and Interpretation:
The final trained SVM classifier delivers accurate predictions about whether a given mushroom is poisonous or edible based on its features. The model provides a reliable tool for identifying mushrooms' potential risks in real-world scenarios, aiding individuals in making informed decisions about consumption.

## Flowchart

![Screenshot_2023-08-29-22-22-30-279-edit_com bezapps flowdiademo](https://github.com/Amirth24/mushroom-classification/assets/97495357/e1a64c68-fa99-4a95-9feb-2b6660e0e800)


## Deployment

In an effort to make the SVM-based mushroom classifier accessible and user-friendly, the model has been successfully deployed using a combination of frontend and backend technologies. This deployment not only ensures the model's availability to a wider audience but also provides a seamless and interactive experience for users seeking to determine the edibility of mushrooms.

### Frontend Development
The frontend of the deployed solution serves as the user interface, allowing individuals to input mushroom characteristics and receive predictions about their edibility. A well-designed and intuitive web application was created to facilitate easy interaction. The frontend likely includes components such as input forms, buttons, and visual elements to guide users through the process.

### Backend Development:
At the core of the deployment lies the backend, where the SVM model's functionality is integrated. The backend is responsible for receiving user inputs from the frontend, processing them, and applying the trained SVM classifier to make predictions. This process involves data preprocessing, feature extraction, and passing the data through the SVM classifier to obtain the prediction result.

### View the Deployment Here:

    https://huggingface.co/spaces/Amirth24/mushroom-classifier

## Screenshots

Here the Screenshots of deployed application

### Home Screen

![IMG_20230829_225130](https://github.com/Amirth24/mushroom-classification/assets/97495357/cd1de596-13b0-449f-bf51-48ebe3d13c53)


### Prediction Screen

![IMG_20230829_225205](https://github.com/Amirth24/mushroom-classification/assets/97495357/85bf699a-eb85-4b46-a670-3cd1c0b04943)

![IMG_20230829_225149](https://github.com/Amirth24/mushroom-classification/assets/97495357/804b371d-b37b-4516-86af-584d5df186e3)


## Documentation

[Support Vector Machine (SVM)](https://scikit-learn.org/stable/modules/svm.html)

[Flask](https://flask.palletsprojects.com/en/2.3.x/)

[HuggingFace](https://huggingface.co/docs)

