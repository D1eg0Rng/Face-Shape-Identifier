# Face-Shape-Finder
![image](https://user-images.githubusercontent.com/122308669/233490995-75416e12-fe68-4b32-8ff9-81c49d32071f.png)

# Business Understanding:
The goal of this project was to help the online eyewear retailer, Zenni Optical, provide a better service to its customers by implementing an AI-powered feature that identifies face shapes. This feature would help customers find the right glasses for their face shape more easily and accurately, improving their overall shopping experience.

![qdoewbrmuei9rtd7h1hm](https://user-images.githubusercontent.com/122308669/233490078-8a485ad3-8784-4148-ba9e-707b6d483bc2.png)
![Screenshot 2023-04-18 141808](https://user-images.githubusercontent.com/122308669/233487495-01920753-3704-4496-a16d-e5a29a36a387.png)

# Data Understanding:
The dataset used for this project was sourced from Kaggle and contains 5000 images of female celebrities categorized according to their face shape - Heart, Oblong, Oval, Round, and Square.

![Kaggle_logo](https://user-images.githubusercontent.com/122308669/233490742-05c48b5c-bf3e-4830-b01f-d452e1e57f3d.png)
![Screenshot 2023-04-19 131642](https://user-images.githubusercontent.com/122308669/233488012-17ff7593-6258-4ff4-9c87-af5dfbe1e69f.png)

# Preprocessing:
The images were preprocessed using the Haar cascade algorithm to detect faces and cropped the detected areas to remove excess noise. Then I tried implementing two different types of edge detection, Canny and Sobel.

![image](https://user-images.githubusercontent.com/122308669/233489471-05cdcbff-54c3-4e9f-a86f-cc99009ce946.png)

# Modeling:
For this image classification task, transfer learning was used, specifically the pre-trained VGG16 model. The model was further enhanced by adding six additional dense layers and dropout layers to avoid overfitting, leading to improved results in experiments. Two approaches were tried to improve the model, Canny and Sobel edge detection, but the Sobel model proved to be the best.

## Model Architecture
![Screenshot 2023-04-19 150043](https://user-images.githubusercontent.com/122308669/233489041-315fb595-31ae-487a-83b5-4ed4950a5766.png)

# Evaluation:
The scores are decent, but there is room for improvement. We can see that the main issue is the misclassification of the Oval class.

![image](https://user-images.githubusercontent.com/122308669/233489997-c3f44d88-59c7-4b90-a594-3d871c0af17f.png)

## Recommendations:

- Add the model to the website, along with a service rating button to track customer satisfaction.
- Continue to add new customer images to the database.

## Next Steps:

- Deploy a demo application using streamlit.
- Develop a recommendation system that recommends specific glasses based on face shape, rather than just a group of glasses.
