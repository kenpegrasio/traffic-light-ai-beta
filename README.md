# 🚦 AI-Driven Traffic Lights with Computer Vision (Beta Version)

Welcome to the beta version of the **AI-driven Traffic Lights with Computer Vision** project! Our aim is to help reduce traffic congestion by dynamically adjusting red and green light durations based on real-time vehicle detection.

## 🔍 How Does It Work?

This project combines the **YOLOv8 model** (from the Ultralytics library) with **OpenCV** to detect and count vehicles approaching the intersection. Using this data, the system adjusts the traffic light duration to allow more vehicles to pass during busy times and reduce unnecessary waiting during quiet periods. 

The setup also includes **Arduino UNO** for prototyping, the **pySerial** library for Serial communication, and **cvzone** library for drawing and labelling. 

To simulate real-life conditions in this prototype, sample photos of traffic situations stored in the `images` folder are used. The program will randomly select an image from the folder, then adjusts the duration of the red and green LEDs based on the traffic density shown in the photo.

Check out the full circuit schema below to try it yourself!

## 🛠️ Getting Started

Here’s a quick guide to help you set up and test the project.

1. **Clone the Repository**

   ```bash
   git clone https://github.com/kenpegrasio/traffic-light-ai-beta.git
   cd traffic-light-ai-beta
2. **Install Dependencies**

   This project requires Python libraries such as `Ultralytics`, `OpenCV`, `pySerial`, and `cvzone`. Install them with:
   
   ```bash
   pip install ultralytics opencv-python pyserial cvzone
4. **Setup the Arduino**
   
   Connect your Arduino UNO as shown in the circuit schema below, then upload the provided Arduino code to get started.

6. **Run the Program**
   
   With everything connected, run the script:
   
   ```bash
   python main.py

Watch as the traffic light changes duration based on real-time vehicle detection!

## 🖥️ Tech Stack

- **YOLOv8**: For vehicle detection and counting.
- **OpenCV**: For image processing and video feed handling.
- **Arduino UNO**: To control the physical traffic light prototype.
- **pySerial**: For Serial communication
- **cvzone**: For convenience in drawing and labelling

## 🗺️ Circuit Schema

_(Refer to the diagram below for your connections)_
![Circuit_Schema](https://github.com/user-attachments/assets/d42fdcd9-b34d-4064-999e-f0f7e0410244)
