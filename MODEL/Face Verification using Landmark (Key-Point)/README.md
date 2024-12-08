# Face Verification Using Landmarks

This repository provides a Python-based implementation for face verification using facial landmarks (keypoints). It employs a step-by-step approach for detecting, aligning, and verifying faces based on normalized facial landmark distances.

---

## Features

1. **Face Detection**  
   Detects faces in images using the Haar Cascade classifier.

2. **Face Alignment**  
   Aligns detected faces using a custom alignment model to normalize facial positioning.

3. **Face Verification**  
   Compares two sets of facial landmarks by calculating the distance between normalized keypoints.

---

## Workflow

The system follows these primary steps:

1. **Input Images**: Accepts two face images as input for verification.  
2. **Face Detection**: Uses Haar Cascade to detect faces in the images.  
3. **Landmark Extraction**: Extracts facial keypoints for each detected face.  
4. **Face Alignment**: Aligns the detected faces for consistency using a custom alignment model.  
5. **Landmark Normalization**: Normalizes extracted landmarks for scale invariance.  
6. **Distance Calculation**: Calculates the Euclidean distance between normalized landmarks of both faces.  
7. **Decision**: Determines whether the faces belong to the same individual based on a predefined threshold.

---

## Prerequisites

To run this project, ensure you have the following dependencies installed:

- Python 3.x
- OpenCV
- NumPy
- Matplotlib (optional, for visualization)

Install the dependencies using the command:

```bash
pip install opencv-python-headless numpy matplotlib
```

---

## Installation and Usage

### Clone the Repository

```bash
git clone https://github.com/your-username/face-verification-landmarks.git
cd face-verification-landmarks
```

### Running the Code

1. Place the two images you want to verify in the `images/` directory.
2. Update the paths to the images in `main.py`.
3. Run the script:

```bash
python main.py
```

### Expected Output

The script will output the following:

1. Aligned faces.
2. Extracted facial landmarks.
3. Distance score between the landmarks.
4. A verification result: "Match" or "No Match."

---


---

## Algorithms and Methods

1. **Face Detection**:  
   - The Haar Cascade classifier detects faces in grayscale images. It is a pre-trained XML file provided by OpenCV.

2. **Face Alignment**:  
   - Aligns faces based on eye positions and other key landmarks, ensuring consistency in pose.

3. **Distance Calculation**:  
   - Uses Euclidean distance between normalized facial landmarks for comparison.  
   - Threshold tuning is required for optimal performance.

---

## Limitations

- **Lighting and Pose Variability**: Performance may degrade in challenging lighting conditions or extreme poses.
- **Accuracy**: The system relies on the accuracy of Haar Cascade and facial landmarks detection, which can vary across datasets.

---

## Future Enhancements

1. Replace Haar Cascade with more robust face detectors like DNN-based models or MTCNN.
2. Introduce machine learning models for dynamic thresholding.
3. Integrate deep learning techniques for improved landmark extraction and verification.

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any feature requests, bugs, or improvements.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments

- [OpenCV](https://opencv.org/) for face detection and computer vision tools.
