# Security Surveillance System for Intruder Detection

A Flask-based application that provides real-time video monitoring with AI-powered intruder detection using YOLOv8.

## Features

- Real-time video streaming from webcam
- Object detection using custom-trained YOLO model
- Automatic image capture when intruders are detected
- Image processing techniques (histogram equalization, edge detection, thresholding)

## Installation

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Setup Before Running

1. Download model weights from [here](https://drive.google.com/file/d/16zYRZZ6x-llVUJFSU5u8zjvQZzTT_leX/view?usp=sharing) and place `best15.pt` in the project directory
2. Delete the `runs` folder if present in your directory
3. Delete all folders ending with `_images` to avoid browser caching issues
4. Verify you have these files in your directory:
   - app.py
   - iptechniques.py
   - best15.pt
   - requirements.txt
   - templates folder
   - logo folder

## Usage

1. Run the application from terminal:
   ```bash
   python app.py
   ```
2. Open your web browser and go to the localhost address shown in the terminal

## Detection Information

This trained model can identify only 4 classes (Arun, Ali, Kaushik and Intruder). Any person other than Arun, Ali, or Kaushik will be classified as an intruder.