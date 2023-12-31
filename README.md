# TinyML Object Classification on ESP32 with Edge Impulse

Welcome to the repository for my TinyML project focused on real-time object classification using Edge Impulse on ESP32 platforms! This project explores the integration of TinyML, particularly a MobileNet V2 model with 96x96 input, and Edge Impulse for efficient object classification.

## Project Overview

In this project, I leveraged the Animals-10 dataset, curating a balanced subset for training the model. The implementation is demonstrated on AI Thinker ESP32-CAM and ESP32-S3 Xiao boards, enhanced with an ST7789 display for real-time visual feedback. 

## Project Link
https://studio.edgeimpulse.com/studio/327359

## Key Features

- Object classification using TinyML and Edge Impulse
- ESP32-CAM and ESP32-S3 Xiao hardware implementation
- Balanced dataset from Animals-10 with additional room images

## Getting Started

To run this project on your ESP32 device, follow these steps:
Schematic:
On AI Thinker ESP32-CAM:
TFT to ESP32CAM:
GND -> GND
VCC -> 3.3V
SCK -> IO14
SDA -> IO13
RES -> IO12
DC  -> IO2
BLK -> 3.3V

on XIAO ESP32S3 Sense:
TFT to ESP32S3 Sense:
GND -> GND
VCC -> 3.3V
SCK -> IO10
SDA -> IO8
RES -> IO3
DC  -> IO2
BLK -> 3.3V

1. Clone this repository: `[git clone https://github.com/fitranurmayadi/Edge-Impulse-ESP32S3-Animals-10-with-ST7789.git]`
2. Install the required dependencies.
   - Arduino IDE.
   - ESP32 Board on Arduino Board Manager.
   - Edge Impulse Project as Libraries (https://studio.edgeimpulse.com/studio/327359), deploy project as Arduino Library with EON Compiler off.
   - Arduino TFT libraries: https://github.com/Bodmer/TFT_eSPI and https://github.com/Bodmer/TFT_eFEX
3. Edit file Setup.h on TFT_eSPI library coresponding to the Schematic.
4. Replace ESP-NN folder in project library. see https://www.hackster.io/mjrobot/tinyml-made-easy-image-classification-cb42ae
5. Upload the code to your ESP32 device.
6. Open the Serial Monitor to view real-time classification results or view on tft display.

## Additional Resources

- [Animals-10 Dataset](https://www.kaggle.com/datasets/alessiocorrado99/animals10)
- [Room Dataset](https://www.kaggle.com/datasets/robinreni/house-rooms-image-dataset)

#Tutorial Reference:

- Introduction to Embedded Machine Learning by Shawn Hymel and Alexander Fred-Ojala: https://www.coursera.org/learn/introduction-to-embedded-machine-learning or https://www.youtube.com/watch?v=TgekTwrftcg&list=PL7VEa1KauMQqZFj_nWRfsCZNXaBbkuurG

- Getting Started with Xiao ESP32S3 Sense: https://wiki.seeedstudio.com/xiao_esp32s3_keyword_spotting/#building-a-mechine-learning-model

- XIAO_ESP32S3-Image_Classification by Marcelo Rovai: https://github.com/Mjrovai/XIAO-ESP32S3-Sense/blob/main/1.XIAO_ESP32S3-Image_Classification.pdf
- https://www.hackster.io/mjrobot/tinyml-made-easy-image-classification-cb42ae


## Contribution
Feel free to contribute, open issues, or provide feedback. Collaboration is highly encouraged!
