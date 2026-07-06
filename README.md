# 🧘 AI Yoga Coach

A real-time AI-powered Yoga Pose Detection and Coaching application built entirely in the browser using **MediaPipe Pose Landmarker** and JavaScript.

The application analyzes the user's body posture through a webcam, compares joint angles against predefined yoga pose templates, provides live corrective feedback, calculates pose accuracy, and guides users through complete yoga sessions with voice assistance.

---

# Features

## Real-Time Pose Detection

- Uses MediaPipe Pose Landmarker
- Detects 33 human body landmarks
- Runs entirely inside the browser
- No backend server required
- No user images are uploaded

---

## Supported Yoga Poses

Currently includes six yoga poses:

- Dandasana
- Plank Pose
- Vajrasana
- Downward Dog
- Tree Pose
- Baddha Konasana

Each pose contains:

- Pose description
- Step-by-step setup instructions
- Target joint angles
- Personalized coaching messages

---

# AI Coaching System

Unlike traditional pose detection systems that highlight every mistake simultaneously, this application uses a **Sequential Coaching Strategy**.

The coach:

1. Detects all incorrect joints
2. Prioritizes the most important correction
3. Gives only one instruction at a time
4. Waits until the user fixes that joint
5. Confirms the correction
6. Praises the user
7. Moves to the next correction

This greatly improves usability and reduces cognitive overload.

---

# Live Feedback

The system provides

- Real-time skeleton visualization
- Joint highlighting
- Live angle comparison
- Pose accuracy score
- Corrective instruction
- Voice coaching
- Progress indicators
- Perfect pose detection

---

# Pose Accuracy

The application compares measured joint angles with predefined reference angles.

Tracked joints include

- Left Shoulder
- Right Shoulder
- Left Elbow
- Right Elbow
- Left Hip
- Right Hip
- Left Knee
- Right Knee
- Left Ankle
- Right Ankle

Each joint has its own allowable threshold.

---

# Guided Yoga Sessions

Users can start an automatic guided session.

The application automatically:

- Loads the next pose
- Reads setup instructions
- Waits for correct execution
- Confirms pose completion
- Advances to the next pose
- Tracks overall progress

---

# Voice Coaching

Uses the Web Speech API.

Voice features include

- Setup instructions
- Live corrections
- Praise messages
- Session guidance
- Voice on/off toggle

---

# Pose Scoring

The application continuously calculates

- Number of joints in correct position
- Percentage accuracy
- Overall pose quality

Visual score indicators include

- Circular progress ring
- Percentage score
- Joint counter
- Color-coded accuracy

---

# Skeleton Visualization

The detected skeleton is drawn directly over the webcam feed.

Features include

- Landmark visualization
- Pose connections
- Highlighted incorrect joints
- Mirrored camera display
- Live updates

---

# Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | User Interface |
| CSS3 | Styling |
| JavaScript (ES6 Modules) | Application Logic |
| MediaPipe Pose Landmarker | Human Pose Detection |
| Web Speech API | Voice Feedback |
| Canvas API | Skeleton Rendering |
| WebRTC | Webcam Access |

---

# Project Structure

```
AI-Yoga-Coach/
│
├── index.html
├── README.md
```

The project is intentionally implemented as a single HTML application that contains

- HTML
- CSS
- JavaScript

for easy deployment.

---

# Pose Detection Pipeline

```
Webcam
      │
      ▼
MediaPipe Pose Landmarker
      │
      ▼
Extract Body Landmarks
      │
      ▼
Calculate Joint Angles
      │
      ▼
Compare With Reference Pose
      │
      ▼
Detect Errors
      │
      ▼
Prioritize Corrections
      │
      ▼
Generate Coaching Feedback
      │
      ▼
Update User Interface
```

---

# Included Yoga Pose Library

Each pose contains:

```
Pose Name

Description

Setup Instructions

Reference Joint Angles

Feedback Messages

Correction Priority
```

---

# Joint Priority Order

Corrections follow this order:

1. Left Knee
2. Right Knee
3. Left Hip
4. Right Hip
5. Left Shoulder
6. Right Shoulder
7. Left Elbow
8. Right Elbow
9. Left Ankle
10. Right Ankle

This prioritization stabilizes the body before correcting smaller movements.

---

# User Interface

The interface contains

### Header

- Logo
- Voice Toggle
- Model Status

### Camera Panel

- Live Webcam
- Skeleton Overlay
- FPS Counter
- Pose Badge
- Perfect Pose Animation

### Sidebar

- Pose Score
- Guided Session
- Pose Selection
- Coach Feedback
- Joint Angles

---

# How It Works

## Step 1

Load MediaPipe Pose model.

## Step 2

Enable webcam.

## Step 3

Select a yoga pose.

## Step 4

The application extracts body landmarks.

## Step 5

Joint angles are calculated.

## Step 6

Angles are compared with reference values.

## Step 7

Incorrect joints are prioritized.

## Step 8

One corrective instruction is spoken.

## Step 9

The system waits until the correction is held.

## Step 10

Praise is given.

## Step 11

The next correction begins.

---

# Browser Requirements

Recommended browsers

- Google Chrome
- Microsoft Edge
- Brave

Requires

- Webcam permission
- JavaScript enabled
- Internet connection (to load MediaPipe)

---

# Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI-Yoga-Coach.git
```

Open the project

```bash
cd AI-Yoga-Coach
```

Run a local server

Python

```bash
python -m http.server
```

or

VS Code Live Server

Then open

```
http://localhost:8000
```

---

# No Backend Required

The application runs completely inside the browser.

No

- Flask
- Django
- Node.js
- Database

is required.

---

# Advantages

- Lightweight
- Fast
- Privacy preserving
- Browser based
- No image upload
- Cross-platform
- Easy deployment
- Real-time performance

---

# Future Improvements

Potential enhancements include

- More yoga poses
- Pose difficulty levels
- AI pose classification
- Personalized training plans
- Workout history
- Progress analytics
- Mobile optimization
- TensorFlow.js integration
- Multi-person detection
- Custom pose creation
- Exercise recommendations
- Fitness dashboard

---

# Limitations

- Single-person detection
- Front-facing camera preferred
- Requires adequate lighting
- Accuracy depends on camera quality
- Uses predefined pose templates

---

# License

This project is intended for educational and research purposes.

---

# Acknowledgements

- Google MediaPipe
- Web Speech API
- HTML5 Canvas
- JavaScript ES6 Modules

---

# Author

Developed as a browser-based AI Yoga Coaching application for real-time pose estimation, intelligent correction, and guided yoga practice.
