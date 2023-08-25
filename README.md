# Object Detection on Instagram Posts with Open CV

Object detection is a computer vision technique that identifies and locates objects in images and videos. It is a powerful tool that can be used for a variety of tasks, such as image classification, scene understanding, and robotics.

Object detection models are typically categorized into two types: single-stage and two-stage. Single-stage models, such as YOLO and SSD, are faster and simpler to train, but they are not as accurate as two-stage models. Two-stage models, such as R-CNN, are more accurate, but they are slower and require more computational resources. The advent of deep neural networks has revolutionized object detection. Deep neural networks are able to learn complex features from images, which allows them to achieve state-of-the-art performance on object detection tasks.
Following is an image which was processed with the MobileNet SSDv2 object detection algorithm.

<img src="https://github.com/aaryan20/Object-Detection-Open-CV/blob/245b4976b15934773fade9c749df8d31901de1b1/image_result.jpg"  width="750" height="900">


In this project we use a pretrained [MobileNet SSDv2](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md), trained on the [MS COCO dataset](https://cocodataset.org/) to make predictions on the scraped posts from instagram.
Here we perform object detection on Instagram handles like keralatourism, rajasthan_tourism etc.

This project can be classified into 3 steps:
1. Scraping Post Data from Instagram
2. Processing JSON files (Post metadata)
3. Image Processing with Object Detection on each post
4. Exporting Dataset

Firstly Instagram data is scraped from various handles, using the instagram_scrape.ipynb notebook.
Then we use the ObjectDetectionCV2.ipynb to process JSON and run Object Detection.
We iteratively loop over the posts collected from the instagram scraper and construct a dataset for further analysis.


A dataset like below is generated, after processing the posts from instagram.


![dataset](https://github.com/aaryan20/Object-Detection-Open-CV/blob/bda1f709e10cc5028f6a677fd164a84267d137dd/dataset.png)



