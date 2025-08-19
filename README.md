# real-life-cover-drive-analysis
🏏 Real-Time Cover Drive Analyzer

This project implements a real-time cricket cover drive analyzer in Python.
It processes an entire video (not just screenshots/frames), performs pose estimation frame by frame, overlays live annotations, and finally outputs an annotated video along with a shot evaluation report.

 Features

1. Real-time video processing – no screenshots, frame exports, or manual intervention.
2. Pose estimation with MediaPipe Pose

 Live overlays:
Skeleton with key joints.
Angles of elbows, shoulders, knees.
Wrist speed graph (to detect impact).
Green/red cues for good/bad posture.
 Final shot evaluation with metrics:
Head stability (steady head = balance).
Front-foot stride (commitment to ball).
Shoulder rotation (open vs closed stance).
Elbow extension (classic high elbow).
Swing plane error (bat path approximation).
Weight transfer (hips over feet).
Impact detection via wrist-speed peak in downswing.
Exports:
Annotated video (.mp4).
JSON report with metrics and verdict.

cover_drive_rt/
│── cover_drive_analyzer.py   # Main system
│── requirements.txt          # Dependencies
│── README.md                 # Documentation
