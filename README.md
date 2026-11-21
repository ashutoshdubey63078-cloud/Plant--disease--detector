# Plant-disease-detector
Plant disease detection using MobileNetV2 transfer learning, classifies 38 leaf disease classes with ~94% validation accuracy. Includes a Gradio demo app. Topics (tags): deep-learning image-classification tensorflow keras transfer-learning plantvillage gradio computer-
# Plant Disease Detector 🌿

Patte ki photo se plant disease pehchanne wala CNN model.

## Overview
- Dataset: PlantVillage (54,305 images, 38 classes)
- Model: MobileNetV2 (ImageNet pretrained) + custom classifier head
- Result: ~94% validation accuracy (5 epochs)

## Tech Stack
Python, TensorFlow/Keras, Gradio, Google Colab

## How it works
1. Images resize to 224x224, data augmentation (flip, rotation)
2. MobileNetV2 as frozen feature extractor
3. GlobalAveragePooling + Dropout + Softmax layer

## Run locally
pip install tensorflow gradio
python app.py

## Limitations
- PlantVillage images lab-style hain; real field photos par accuracy kam ho sakti hai
- Sirf 38 classes supported

## Future work
- Fine-tuning, field-condition images, mobile app deploymen
