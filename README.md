# Chidera_VisionAI_Project

This project aims to create a robust dataset for YOLO-based object detection and classification by leveraging IMDb's comprehensive collection of animated show thumbnails.
![image](https://github.com/user-attachments/assets/a08cc709-edab-4b0e-a179-9c62b4adfe9d)


## Steps and Workflow
*Data Collection*

Use IMDb to retrieve images for animated shows.
Manually select 500 images, 50 for each of the 10 shows want to use.
Format the downloaded images as PNG or JPG files.

*Data Organization*

Organize 500 images into 10 folders based on their corresponding television show.

*Preprocessing*

Resize and normalize the images to align with YOLO's requirements.

*Dataset Upload*

Use Ultralytics: Roboflow to upload the dataset and label the images.

*Class Annotation and Boundary Box*

Label classes based on the show names to simplify the classification task.
Use Roboflow's auto-annotate feature initially. 
This step helps with 20% of the boundary boxes but is imperfect, and cross-checking is needed.
For best results, manually correct and update annotations on all 500 images.

*Train the YOLO model on the labeled dataset*

Use appropriate GPU-enabled environments like Google Colab for efficient training.
Track training metrics such as precision, recall, and mAP to evaluate the model.

*Test model on seen & unseen data*

Evaluate performance in terms of accuracy in class (show_name) identification.
Try to conduct error analysis to identify and address common misclassifications.

*Expected Outcome*

I expect the YOLO model to be capable of accurately detecting and classifying animated shows based on their network of origin.
