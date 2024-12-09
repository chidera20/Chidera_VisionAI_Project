# Chidera_VisionAI_Project

This project aims to create a robust dataset for YOLO-based object detection and classification by leveraging IMDb's comprehensive collection of animated show thumbnails.
![image](https://github.com/user-attachments/assets/a08cc709-edab-4b0e-a179-9c62b4adfe9d)


## Steps and Workflow
*Data Collection*

Use IMDb to retrieve images for animated shows. https://www.imdb.com/?ref_=nv_home
Manually select 500 images, 50 for each of the 10 shows want to use.
Format the downloaded images as PNG or JPG files.

*Data Organization*

Organize 500 images into 10 folders based on their corresponding television show.

*Dataset Upload*
![image](https://github.com/user-attachments/assets/35e9ffcd-7886-4f8f-b8bd-ac1b4c33ebf5)

Use Ultralytics: Roboflow to upload the dataset and label the images.

*Preprocessing*
![image](https://github.com/user-attachments/assets/82527819-0fc7-41ed-b3b1-1dce965556e2)

Resize and normalize the images to align with YOLO's requirements.

*Class Annotation and Boundary Box*
![image](https://github.com/user-attachments/assets/8702e395-1777-4943-9e51-f8d8695952ab)

Label classes based on the show names to simplify the classification task.
Use Roboflow's auto-annotate feature initially. 
This step helps with 20% of the boundary boxes but is imperfect, and cross-checking is needed.
For best results, manually correct and update annotations on all 500 images.

*Train the YOLO model on the labeled dataset*
![image](https://github.com/user-attachments/assets/7f791997-ba48-4b6b-aa63-88bf96a63d8b)

Use appropriate GPU-enabled environments like Google Colab for efficient training.
![image](https://github.com/user-attachments/assets/4d08f06b-e200-449d-b60a-f31dd3be53d4)

Track training metrics such as precision, recall, and mAP to evaluate the model.
![image](https://github.com/user-attachments/assets/70675beb-b3b2-4701-9c6f-bcba3013943f)

*Test model on seen & unseen data*
![image](https://github.com/user-attachments/assets/2872b9fd-95da-4f4d-824e-60ecfd377521)

Evaluate performance in terms of accuracy in class (show_name) identification.
![image](https://github.com/user-attachments/assets/b00a11c0-3627-42ed-af9e-b316bdd1facd)

Try to conduct error analysis to identify and address common misclassifications.

*Expected Outcome*

I expect the YOLO model to be capable of accurately detecting and classifying animated shows based on their network of origin.
