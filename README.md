# Car & Traffic Scene Intelligence System

An advanced computer vision application that detects vehicles, traffic signals, and people in urban traffic scenes. It provides specific visual alerts (color-coded rectangles) and statistical counts to assist in traffic management and analysis.

## 📁 Repository Contents

* **`car_color_working.ipynb`**: The research notebook detailing the model training pipeline, traffic dataset preparation, and performance evaluation metrics.
* **`app.py`**: A production-ready Streamlit application that provides a GUI for image uploads, live inference, and intelligent scene rendering.
* **`requirements.txt`**: A comprehensive list of dependencies and packages required for the environment.
* **`packages.txt`**: A list of system-level packages required for specialized support (such as video codecs and OS-level libraries).

## 🚀 Features

* **Intelligent Object Detection**: Identifies Cars, Traffic Lights, and People using YOLO-based architectures.
* **Custom Color Classification**: Implements logic to distinguish car colors and apply visual filters:
* **Red Rectangles**: Applied specifically to blue-colored cars.
* **Blue Rectangles**: Applied to all other vehicle colors.


* **Scene Analytics**: Automatically calculates and displays the count of vehicles and pedestrians in the scene.
* **Intuitive UI**: Allows users to upload images and receive real-time processed visual feedback.

## 🔧 Setup & Installation

### 1. Prerequisites

Clone this repository:

```bash
git clone https://github.com/KVAlwaysLearning/Car_Color_Detection_Sub
cd Car_Color_Detection_Sub

```

### 2. Install Dependencies

Install all required libraries and system packages:

```bash
pip install -r requirements.txt
# If deploying on Linux environments:
sudo apt-get install -y $(cat packages.txt)

```

**Key Packages:**

* `streamlit`: For the web user interface.
* `ultralytics`: For YOLO object detection inference.
* `opencv-python`: For image processing and drawing visual annotations (rectangles/labels).
* `gdown`: For automated downloading of pre-trained model weights from Google Drive.

### 3. Model Initialization

The application downloads necessary YOLO model weights (e.g., `yolov8n.pt`, `yolo26n.pt`) automatically upon the first run into the root directory. Ensure your environment has sufficient permissions to write these files.

## 💻 Usage

### Running the App

Launch the web interface locally:

```bash
streamlit run app.py

```

### Exploring the Research

You can open `car_color_working.ipynb` in your preferred Jupyter environment (VS Code, JupyterLab, or Google Colab) to inspect the model training logic, confusion matrices, and validation results.

## 📂 Project Structure

```text
├── app.py             # Streamlit web application
├── car_color_working.ipynb # Research and training notebook
├── requirements.txt   # Python dependencies
├── packages.txt       # System-level dependencies
└── README.md          # Project documentation

```

## 🔗 Links

* **Live App**: [Traffic Intelligence App](https://carcolordetectionsub-app-working.streamlit.app/)
* **GitHub Repo**: [Car & Traffic Detection Repository](https://github.com/KVAlwaysLearning/Car_Color_Detection_Sub)

## **Visuals:**

<img width="1283" height="582" alt="App_1" src="https://github.com/user-attachments/assets/92cdf74c-75f0-4d49-9f43-ce4f80d0a56f" />

<img width="1328" height="613" alt="App_2" src="https://github.com/user-attachments/assets/332c9b5e-8fa9-47ab-9c21-c02470ad7a0d" />

