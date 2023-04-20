# Face-Shape-Identifier

# Business Understanding:
The goal of this project was to help the online eyewear retailer, Zenni Optical, provide a better service to its customers by implementing an AI-powered feature that identifies face shapes. This feature would help customers find the right glasses for their face shape more easily and accurately, improving their overall shopping experience.

![qdoewbrmuei9rtd7h1hm](https://user-images.githubusercontent.com/122308669/233487634-88a5a8d8-0050-4cc1-aa3a-528a3ab5881d.png)
![Screenshot 2023-04-18 141808](https://user-images.githubusercontent.com/122308669/233487495-01920753-3704-4496-a16d-e5a29a36a387.png)


# Data Understanding:
The dataset used for this project was sourced from Kaggle and contains 5000 images of female celebrities categorized according to their face shape - Heart, Oblong, Oval, Round, and Square.

# Preprocessing:
The images were preprocessed using the Haar cascade algorithm to detect faces and cropped the detected areas to remove excess noise.

# Modeling:
For this image classification task, transfer learning was used, specifically the pre-trained VGG16 model. The model was further enhanced by adding six additional dense layers and dropout layers to avoid overfitting, leading to improved results in experiments. Two approaches were tried to improve the model, Canny and Sobel edge detection, but the Sobel model proved to be the best.

# Evaluation:
The model achieved decent results, but there is still room for improvement, particularly in the misclassification of the Oval class with 61% accuracy on validation and 84% on the test.

# Recommendations:

- Add the model to the website, along with a service rating button to track customer satisfaction.
- Continue to add new customer images to the database.

Next Steps:

- Deploy a demo application using streamlit.
- Develop a recommendation system that recommends specific glasses based on face shape, rather than just a group of glasses.
