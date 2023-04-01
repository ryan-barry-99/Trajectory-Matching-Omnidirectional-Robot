# Balloon Trajectory Matching Omnidirectional Robot using YOLO

This project is designed to track a balloon using a custom YOLO model and a 3-wheeled omnidirectional drive robot, which can move in any direction without having to turn. The goal is to punch the balloon back into the air using the robot.

# Dataset and Model

The YOLOv8 model was trained on the V2 Balloon Detection dataset (https://www.kaggle.com/datasets/vbookshelf/v2-balloon-detection-dataset), resulting in efficient real-time detections at high accuracies. The model was trained using PyTorch, and the best weights were saved to the included yolov8_weights.pt file.

# Hardware Compatibility

For compatibility with DepthAI and OpenCV AI Kit hardware, the model must be saved in the Luxonis MyriadX Blob format. To achieve this, the weights were converted to the OpenVINO format using http://tools.luxonis.com/, and then the OpenVINO files were converted to the blob format using http://blobconverter.luxonis.com/.
