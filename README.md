# AWS Rekognition Image Labels Generator

## Overview ☁️
This project is an image labels generator built using Amazon Rekognition. It allows you to recognize and label images automatically. For example, if you upload a photo of a cat, Amazon Rekognition will identify and label the image as a cat.

## Features
- Detects and labels objects in images stored in Amazon S3
- Displays detected labels and confidence scores
- Visualizes bounding boxes for detected objects using Matplotlib

## Steps to Get Started 👩‍💻
1. **Create an Amazon S3 Bucket**
   - Store your images in an S3 bucket for processing.
2. **Upload Images to S3**
   - Add your images to the S3 bucket you created.
3. **Install and Configure AWS CLI**
   - Set up the AWS CLI to interact with AWS services.
   - Run `aws configure` to set your credentials.
4. **Install Required Libraries**
   - Install dependencies:
     ```bash
     pip install boto3 matplotlib pillow
     ```
5. **Import Libraries**
   - The script imports `boto3`, `matplotlib`, and `Pillow` for AWS interaction and image processing.
6. **Add `detect_labels` Function**
   - This function detects labels in images stored in S3 and displays bounding boxes.
7. **Add `main` Function**
   - The main function sets the image and bucket, calls `detect_labels`, and prints the results.
8. **Run the Python File**
   - Execute the script:
     ```bash
     python aws-rekognition-label-images.py
     ```

## Services Used 🛠
- **Amazon S3**: Stores images for label generation.
- **Amazon Rekognition**: Analyzes images and generates labels.
- **AWS CLI**: Interacts with AWS services from the command line.

## Example Usage
Update the `photo` and `bucket` variables in the script to match your S3 image and bucket names. Run the script to see detected labels and bounding boxes visualized on your image.

---

Feel free to customize and extend this project for your own image recognition needs!