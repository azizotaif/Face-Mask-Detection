# Face Mask Detection

In this project I trained, evaluated, and used YOLOv7 on images and videos to detect faces and classify if they're wearing face masks or not, not only that, the model can tell if a face mask is not worn correctly.

## Dataset
The dataset contains 853 images belonging to 3 classes:
- with_mask
- without_mask
- mask_weared_incorrect

[Download Dataset](https://drive.google.com/drive/folders/1kDgOxGBDiNBX0Lz8s0EoFCNOQvgoRilT?usp=sharing)

## Trained Model
[Download Trained Model](https://drive.google.com/file/d/1sbCs61-e6h11D0q7e_UiVwtdyNF0U_KN/view?usp=sharing)

## Code
All preprocessing, training, evaluation, and inference code and details are provided in the notebook above (Face_Mask_Detection.ipynb)

## Inference
To use the model on your own data, follow these steps:
- Download the trained model from  [here](https://drive.google.com/file/d/1sbCs61-e6h11D0q7e_UiVwtdyNF0U_KN/view?usp=sharing)
- Clone YOLOv7 repository and install the requirements
``` shell
git clone https://github.com/WongKinYiu/yolov7.git
pip install -r yolov7/requirements.txt
```
-  Run inference script and modify these parameters according to your data

--source : path to image/video

--weight : path to the trained model

--conf : confidence threshold, the trained model's optimal threshold is 0.26

--name : path to a folder to save results in
``` shell
python ./yolov7/detect.py --source ./yolov7/data/test/images --weight ./runs/train/yolov7x_results8/weights/best.pt --conf 0.26 --name test_images
```
## 🔗 Contact
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:otaif.abdulaziz@gmail.com)
[![Linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdulazizotaif)
