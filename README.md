# Face-Shape-Identifier

# Business Understanding:
The goal of this project was to help the online eyewear retailer, Zenni Optical, provide a better service to its customers by implementing an AI-powered feature that identifies face shapes. This feature would help customers find the right glasses for their face shape more easily and accurately, improving their overall shopping experience.

![qdoewbrmuei9rtd7h1hm (1)](https://user-images.githubusercontent.com/122308669/233489668-e964fad3-0cfe-421a-a364-065373ab4d10.png)
![Screenshot 2023-04-18 141808](https://user-images.githubusercontent.com/122308669/233487495-01920753-3704-4496-a16d-e5a29a36a387.png)

# Data Understanding:
The dataset used for this project was sourced from Kaggle and contains 5000 images of female celebrities categorized according to their face shape - Heart, Oblong, Oval, Round, and Square.

![png-transparent-kaggle-predictive-modelling-data-science-business-predictive-analytics-数据-blue-text-laboratory-thumbnail](https://user-images.githubusercontent.com/122308669/233488086-9a0af328-f903-477a-abb8-d5315131c625.png)
![Screenshot 2023-04-19 131642](https://user-images.githubusercontent.com/122308669/233488012-17ff7593-6258-4ff4-9c87-af5dfbe1e69f.png)

# Preprocessing:
The images were preprocessed using the Haar cascade algorithm to detect faces and cropped the detected areas to remove excess noise. Then I tried implementing two different types of edge detection, Canny and Sobel.

![image](https://user-images.githubusercontent.com/122308669/233489471-05cdcbff-54c3-4e9f-a86f-cc99009ce946.png)

# Modeling:
For this image classification task, transfer learning was used, specifically the pre-trained VGG16 model. The model was further enhanced by adding six additional dense layers and dropout layers to avoid overfitting, leading to improved results in experiments. Two approaches were tried to improve the model, Canny and Sobel edge detection, but the Sobel model proved to be the best.

## Model Architecture
![Screenshot 2023-04-19 150043](https://user-images.githubusercontent.com/122308669/233489041-315fb595-31ae-487a-83b5-4ed4950a5766.png)

# Evaluation:
The model achieved decent results, but there is still room for improvement, particularly in the misclassification of the Oval class with 61% accuracy on validation and 84% on the test.

![image](https://user-images.githubusercontent.com/122308669/233489997-c3f44d88-59c7-4b90-a594-3d871c0af17f.png)

# Recommendations:

- Add the model to the website, along with a service rating button to track customer satisfaction.
- Continue to add new customer images to the database.

Next Steps:

- Deploy a demo application using streamlit.
- Develop a recommendation system that recommends specific glasses based on face shape, rather than just a group of glasses.
