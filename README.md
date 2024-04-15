# exercise_detection_reps
AI Code to Recognize Exercises and Count Reps.
For exercise recognition, we utilized the OpenVINO action_recognition_0001 pre-trained model. Subsequently, we integrated a customized logic layer to specifically identify actions classifiable as exercises.
To count repetitions, we employed MediaPipe to identify Body Landmarks. Using these landmarks, we calculated joint angles and assessed positions (Extension & Contraction) to count repetitions accurately.
Finally, with the CV2 library, we captured frames and displayed the results obtained from the model.
As an additional feature, the code can save the analyzed frames and make a video out of them.

## Features
- Detects and tracks 4 types of exercises: Situps, Push ups, Squats and Pull ups
- Counts repetitions for each exercise.
- Supports both real-time camera input and video file analysis.
- Real-time exercise recognition and repetition counting.
- Record and save as video the analyzed frames.

## Installation
1. Download the IPYNB file code_ex_detection.ipynb.
2. Install the required Python dependencies:
pip install -r requirements.txt
3. Open the IPYNB on Anaconda and follow the instructions in the notebook.

## Demo
https://github.com/aldemarp93/exercise_detection_reps/assets/131469036/a5eb57ee-6704-4405-af48-16e70759063c



## Acknowledgements
- The exercise detection and tracking algorithm is based on [OpenCV](https://opencv.org/) and [TensorFlow](https://www.tensorflow.org/).
- The repetition counter and Landmark detection comes from MediaPipe.
