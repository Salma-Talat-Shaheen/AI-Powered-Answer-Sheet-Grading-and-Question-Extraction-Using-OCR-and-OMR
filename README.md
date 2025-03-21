# Questionnaire Analysis System
<p align="center">
  <img src="https://github.com/Salma-Talat-Shaheen/AI-Powered-Answer-Sheet-Grading-and-Question-Extraction-Using-OCR-and-OMR/blob/main/Images_Smaples/InputToOutput.png?raw=true" alt="Alt Text" width="600"/>
</p>


##  `► Table of Contents ◄`
1. [Introduction :](#introduction)
2. [Methodology :](#methodology)
3. [Results :](#results)
4. [Comments :](#comments)
5. [Conclusion :](#conclusion)
6. [References :](#references)

---

### `✦ Introduction`

In a digital world, simplifying data collection is essential. This **Questionnaire Analysis System** automates the process of scanning, detecting, and evaluating answers from filled-out questionnaires. 

Once the questionnaires are scanned and uploaded, the system automatically detects the marked answers, generates question IDs, and calculates results — all without any manual input, saving time and reducing errors. 

---

### `✦ Methodology`

#### 1. Designing the Questionnaire
A multiple-choice questionnaire template was created. Users manually fill out the form by marking answers with a pen.

#### 2.  Scanning & Preprocessing the Image
Once filled out, the form is scanned and saved as an image. The system preprocesses the image to enhance quality for better detection.

#### Preprocessing Steps:
- **Grayscale**: Simplifies the image.
- **Blurring**: Reduces noise.
- **Edge Detection**: Highlights the marked answers.
- **Orientation Correction**: Fixes any tilt or skew.

#### 3.  Extracting Questions & Answers
- **OCR** (Optical Character Recognition) extracts text from the scanned image using `pytesseract`.
- Regular expressions are used to organize questions and answers.

#### 4.  Answer Detection
Contours are detected to identify marked answers, then the answers are compared to a predefined key to calculate scores.

#### 5.  Displaying Results
The answers are displayed in a table, showing which answers were correct, along with a score and feedback (e.g., "Great job!" or "Needs improvement").

---

### `✦ Results`

The system performs efficiently in detecting marked answers and automating grading. Here's how it performed in different test cases:

**`Test Case 1:`**  
✔️ The system detected all answers correctly, resulting in a perfect score.  
 **Output:** <p align="center">
  <img src="https://github.com/Salma-Talat-Shaheen/AI-Powered-Answer-Sheet-Grading-and-Question-Extraction-Using-OCR-and-OMR/blob/main/Images_Smaples/Test1_output.png" alt="Alt Text" width="600"/>
</p>

**`Test Case 2:`**  
❌ The system detected a few answers, resulting in a score of 20%.  
 **Output:** <p align="center">
  <img src="https://github.com/Salma-Talat-Shaheen/AI-Powered-Answer-Sheet-Grading-and-Question-Extraction-Using-OCR-and-OMR/blob/main/Images_Smaples/Test2_output.png" alt="Alt Text" width="600"/>
</p>

**`Test Case 3:`**  
✅ Most answers were detected correctly, leading to a score of 60%.  
**Output:** <p align="center">
  <img src="https://github.com/Salma-Talat-Shaheen/AI-Powered-Answer-Sheet-Grading-and-Question-Extraction-Using-OCR-and-OMR/blob/main/Images_Smaples/Test3_output.png" alt="Alt Text" width="600"/>
</p>


---

### `✦ Comments`

- **Pre-processing**: Improves image quality for better answer detection.
- **Contour Detection**: Identifies marked answers by detecting contours.
- **Answer Extraction**: Compares answers with a predefined answer key.
- **Output**: Visualizes correct and incorrect answers for feedback.
- **Efficiency**: Automates grading and improves accuracy.
- **Future Work**: Improve error handling and support more layouts.

---

### `✦ Conclusion`

The **Questionnaire Analysis System** automates the process of detecting, extracting, and grading answers from scanned questionnaires. By using image processing techniques like OCR and edge detection, it improves accuracy and reduces manual effort, making it an efficient tool for educational assessments and surveys.

---

### `✦ References`

- [Python Code for OMR Answer Sheet Evaluation Using Deep Learning](https://www.youtube.com/watch?v=umSRR2qUKXA)
- [Optical Mark Recognition (OMR)](https://github.com/rbaron/omr)
- [Bubble Sheet Multiple Choice Scanner and Test Grader Using OMR, Python, and OpenCV](https://pyimagesearch.com/2016/10/03/bubble-sheet-multiple-choice-scanner-and-test-grader-using-omr-python-and-opencv)
- [Use pytesseract OCR to Recognize Text from an Image](https://stackoverflow.com/questions/37745519/use-pytesseract-ocr-to-recognize-text-from-an-image)
- [Tables — Rich 13.6.0 Documentation](https://rich.readthedocs.io/en/stable/tables.html)

---

###  **Thank you!**
