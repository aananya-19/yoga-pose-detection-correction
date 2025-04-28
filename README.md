# Yoga Pose Detection and Correction

This project is based on a novel graph-based deep learning approach, YogaPoseGNN, for the accurate classification of yoga asanas using human pose keypoints represented as graphs. YogaPoseGNN models the human skeleton as a graph and uses Graph Attention Networks (GATs) to capture both local and global posture features. By connecting non-adjacent joints, it better distinguishes similar poses, achieving 98.51% testing accuracy and a 0.9851 F1 score. We also built a real-time Pose Correction System that gives subtle feedback based on angle differences, helping users adjust safely during their practice.

# Basic Theory

In our work, we present a real-time yoga pose detection and correction system powered by Graph Neural Networks (GNNs). By modeling body keypoints as a structured graph and introducing higher-order connections between non-adjacent joints, our system captures both local and global posture features, enabling more robust, dynamic, and interpretable pose recognition.

# Dataset

The dataset consists of 1,550 images across five yoga poses— "plank", "warrior2", "goddess", "tree", and "downdog" — split into 1,080 training and 470 testing images in various formats (.jpg, .png, .jpeg, .bmp). The images include diverse lighting, backgrounds, body orientations, and angles, simulating real-world conditions. The dataset was split into training and testing subsets with a 70:30 ratio, resulting in 1,080 training images and 470 testing images.

# GNN-based Yoga Pose Detection System

The Yoga Pose Detection system makes real-time yoga practice easy and interactive. When users launch the app, a simple Tkinter window lets them pick a pose—like goddess, downdog, plank, warrior2, or tree—from a dropdown list. After clicking “Start Camera,” the webcam opens, showing a live video feed alongside a reference image of the selected pose. Using MediaPipe and a trained GNN model, the system processes the video frames and overlays the predicted pose in real time, giving users instant feedback and helping them improve their form on the spot.

# Corrective Feedback System

The angle-heuristics corrective feedback system gives real-time guidance by overlaying pose landmarks, joint connections, and color-coded feedback right onto the live video feed. Users can easily understand how to adjust their posture through clear visual and text prompts. If the system can’t detect any landmarks—like when the user moves out of frame—it gently prompts them to reposition. This setup makes the practice feel more interactive and helps users correct themselves without needing constant supervision.



