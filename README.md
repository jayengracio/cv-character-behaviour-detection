# Real-time Object Detection & Action Recognition For League of Legends Character

### About
My final year project using object detection to recognize a game character and classify their in-game actions (auto-attacks and ability casts) frame-by-frame from gameplay video. Built a synthetic data generation pipeline that programmatically composited masked character/ability sprites onto game map backgrounds with randomized scale, rotation, transparency, and noise to auto-generate a labelled training dataset, removing the need for manual annotation. Trained a YOLOv5 object detection model on this dataset and deployed it (via ONNX + OpenCV DNN) for real-time inference on video.

### Prerequisites:
- Python 3 or higher
- Use of Python Virtual Environment is recommended

### Requirements:
- Install necessary modules from requirements.txt:
```
pip install -r requirements.txt
```

### Set up Virtual Environment (Windows):
In the project's root directory, create a virtual env using command:
```
python -m venv .venv
```
Activate virtual environment:
```
.venv\Scripts\activate
```

### Frameworks and Tools:
- [YOLOv5](https://github.com/ultralytics/yolov5) - Object Detection Algorithm and Model
- [Google Collab Environment](https://colab.research.google.com/github/ultralytics/yolov5/blob/master/tutorial.ipynb) - Cloud Environment for Training
- [Teemo.GG](https://teemo.gg/) - Character Model Viewer
- [MakeSense.AI](https://www.makesense.ai/) - Photo Labeling
- [OBS](https://obsproject.com/) - Video Recording
- [gen_synthetic_images](https://github.com/Oleffa/LeagueAI) - Adapted script for educational use

### Output Showcase:
Below are example video outputs derived from models produced within YOLOv5 framework, utilizing synthetic datasets generated via the methodologies and tools employed within this project.
- https://youtu.be/pNl-ff0ccMc - Early Iteration
- https://youtu.be/qal6MQ1nH_c - Intermediate Iteration
- https://youtu.be/qYYFRdbaEtI - Late Iteration
