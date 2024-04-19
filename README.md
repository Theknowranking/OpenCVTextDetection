# Text Detection using EAST (Efficient and Accurate Scene Text Detector)
This repository contains a Python script for detecting text in images using the EAST (Efficient and Accurate Scene Text Detector) model. The EAST model is trained to detect text in natural scene images with high efficiency and accuracy.

**Requirements**
* Python 3.x
* OpenCV
* NumPy
* imutils

**Usage**
1. Clone the repository to your local machine:
git clone https://github.com/your-username/your-repository.git
2. Download the pre-trained EAST text detection model (frozen_east_text_detection.pb) from [here](https://github.com/oyyd/frozen_east_text_detection.pb) and place it in the root directory of the repository.
3. Place the image you want to perform text detection on in the root directory of the repository and rename it to photo.jpg.
4. Run the cells in Google Colab:
5. The last cell will display the original image with bounding boxes drawn around the detected text regions.

**Explanation**

The script first loads the image (photo.jpg) and resizes it to a fixed size for processing.
It then loads the pre-trained EAST model and forward passes the image through the network to obtain text detection predictions.
Non-maximum suppression is applied to remove redundant bounding boxes.
Finally, the script draws bounding boxes around the detected text regions on the original image and displays it.

**Example**

![download](https://github.com/Theknowranking/OpenCVTextDetection/assets/54183267/5b867192-7e5a-47ec-9ca1-2b7a00663a9f)
![download (1)](https://github.com/Theknowranking/OpenCVTextDetection/assets/54183267/047ca585-f89a-4cc4-b84d-0ed4aa580d89)

**References**
* [EAST: An Efficient and Accurate Scene Text Detector](https://arxiv.org/abs/1704.03155)
* OpenCV: EAST text detection
* [GitHub: oyyd/frozen_east_text_detection.pb](https://github.com/oyyd/frozen_east_text_detection.pb)
