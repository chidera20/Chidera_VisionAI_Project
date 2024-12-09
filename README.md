# Chidera_VisionAI_Project
Project Description
This project aims to create a robust dataset for YOLO-based object detection and classification by leveraging IMDb's comprehensive collection of animated show thumbnails.

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
Label classes based on the show names to simplify the classification task.

*Train the YOLO model on the labeled dataset*
Use appropriate GPU-enabled environments like Google Colab for efficient training.
Track training metrics such as precision, recall, and mAP to evaluate the model.

*Test model on seen & unseen data*
Evaluate performance in terms of accuracy in class (show_name) identification.
Try to conduct error analysis to identify and address common misclassifications.

*Expected Outcome*
I expect the YOLO model to be capable of accurately detecting and classifying animated shows based on their network of origin.
