# AI-Football-Analysis
This project presents an AI Sports Analyst System designed to detect and track important objects in football video and images
The system combines YOLOv8 for object detection with DeepSORT for
multi-object tracking and uses a Gradio dashboard to provide an interactive interface for uploading sports
images and viewing detection results. The supplied outputs show detections of players and referees,
confidence scores, a confusion matrix, and dashboard-level interaction. The project demonstrates how
computer vision can transform raw sports footage into structured observations that support analysis,
review, and future statistical services
# Problem Statement
The problem is to automatically identify and follow sports objects in football images and video despite
changes in scale, camera position, background complexity, motion, and partial occlusion. A useful system
must not only detect objects but also present the outputs in a way that is understandable to a user. The
project therefore combines visual inference, tracking, result rendering, and an interactive dashboard
# Related Work
Modern sports-analytics systems commonly combine object detection, multi-object tracking, and
domain-specific analysis. YOLO-family detectors are widely used because they perform object localization
and classification in a single inference pipeline, making them suitable for near-real-time applications [1].
DeepSORT extends tracking-by-detection by associating detections across frames using motion and
appearance information [2]. OpenCV provides the image and video-processing functions required to read
frames, manipulate visual data, and write annotated outputs [3].
# Dataset
The supplied project outputs indicate a football-focused dataset with the classes player, referee, and
background; the confusion-matrix visualization also displays a football label. The images show
broadcast-style football scenes with multiple players, a referee, a pitch, stadium seating, advertising
boards, and scoreboard overlays. These conditions are useful for testing object detection under realistic
visual clutter.
Dataset documentation note. The provided materials do not state the exact number of images, the
train/validation/test split, the source dataset name, or the number of annotated instances per class. These
values should be added from the training notebook or dataset export before an official submission if they
are available.
