
# Automated Car Parking Using Machine Learning

**Automated Car Parking Using Machine Learning** is a project that aims to efficiently detect and recognize license plates for automated parking systems using computer vision techniques and Optical Character Recognition (OCR). The system detects car license plates with high accuracy and extracts the vehicle information for automated parking management.

## Features
- **License Plate Detection**: Detects vehicle license plates using image processing and machine learning techniques.
- **License Plate Recognition**: Extracts text from the license plates using OCR (Optical Character Recognition) and Tesseract.
- **High Accuracy**: Improved license plate recognition accuracy by 92%.
- **Real-time Processing**: Capable of processing live video streams or static images for vehicle detection.
  
## Technologies Used
- **OpenCV**: Used for image processing and real-time computer vision tasks.
- **Tesseract**: OCR engine used to recognize text from images.
- **OCR (Optical Character Recognition)**: For extracting text from the detected license plates.
  
## Contribution
- **Enhanced License Plate Detection Accuracy**: Improved detection accuracy by 92% using optimized image preprocessing and OCR techniques.
  
## Prerequisites
Before running the project, ensure the following dependencies are installed:
- **Python 3.x**
- **OpenCV**
- **Tesseract-OCR**
- **Pytesseract** (Python wrapper for Tesseract)

## Setup & Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Clean8876/Automated-car-parking-using-ml.git
   cd Automated-car-parking-using-ml
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Install Tesseract-OCR:
   - **Windows**: Download and install from [here](https://github.com/tesseract-ocr/tesseract).
   - **Linux**: Install via the package manager:
     ```bash
     sudo apt-get install tesseract-ocr
     ```

4. Set up the path to Tesseract executable (if needed):
   ```python
   pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'  # Example for Windows
   ```

## Running the Project

1. Run the script to detect and recognize license plates:
   ```bash
   python license_plate_detection.py
   ```

2. The system will:
   - Capture an image from a video feed or static input.
   - Detect the license plate region using OpenCV.
   - Recognize and extract the text from the license plate using Tesseract OCR.
   - Display the detected license plate and extracted text.

## Directory Structure
```
automated-car-parking-using-ml/
├── models/                     # Pre-trained models for license plate detection
├── data/                       # Sample images and video streams
├── scripts/                    # Scripts for detection and recognition
│   ├── license_plate_detection.py  # Main script for detecting and recognizing license plates
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

## Demo
- A real-time video demonstration of the system is available [here](demo_link).
- Sample images showing license plate detection and recognition can be found in the `data/` directory.

## Future Improvements
- Integration with a parking management system for automated ticket generation.
- Optimization for faster real-time processing using GPU acceleration.

## Contributing
If you would like to contribute to this project, follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to reach out for any questions or improvements!

High-Level Design Considerations:
1. System Architecture:
Component Modularization: 
o	Design modular components for image processing, OCR, database interaction, and user interface (if applicable).
o	Modularization improves code maintainability and allows for easy updates or replacements of specific functionalities.
2. Image Processing Module:
Algorithm Selection: 
o	Choose advanced image processing algorithms for improved number plate detection under various conditions.
o	Consider adaptive thresholding, noise reduction, and edge detection techniques.

3. OCR Module:
Algorithm and Configuration: 
o	Select the OCR algorithm and configurations that provide accurate character recognition.
o	Implement pre-processing steps to optimize images for OCR.

4. Database Interaction:
Error Handling: 
o	Implement robust error-handling mechanisms for database connections and operations.
o	Ensure graceful handling of potential issues like connection failures.

5. User Interface (if applicable):
PyQt Integration: 
o	If implementing a user interface, integrate PyQt for an interactive and user-friendly experience.
o	Design features for image selection, displaying results, and user feedback.
6. Logging and Documentation:
Logging System: 
o	Introduce a logging system to record system events, successful detections, and errors.
Documentation: 
o	Use tools like Sphinx or Doxygen to generate code documentation.
o	Maintain detailed documentation for system architecture, module functionalities, and code usage.


7. Testing and Validation:
Test Suites: 
o	Develop comprehensive test suites covering various scenarios, including different image conditions and potential errors.
o	Perform unit testing, integration testing, and system testing.



Brief Analysis of the Existing System:
1.	Strengths: 
o	Successfully integrates image processing, OCR, and database connectivity.
o	Utilizes OpenCV and PyTesseract for efficient image processing and OCR.
o	Establishes MySQL database connections for data logging.
2.	Areas for Improvement: 
o	Error Handling: Strengthen error handling, especially for database operations, to ensure graceful handling of potential issues.
o	Modularization: Further modularize the code for improved maintainability and readability.
o	User Interface: If applicable, consider enhancing the user interface for better user interaction.
