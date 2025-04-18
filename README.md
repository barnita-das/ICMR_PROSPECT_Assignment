### ICMR PROSPECT Phase-1 Assignment

Submitted by:** Barnita Das  
**Role Applied:** Project Research Scientist-I  
**Project Title:** “An endoscopic ultrasound image-based Prediction and Risk Observation System for Chronic Pancreatitis Evaluation using Convolutional Neural Network Technique (PROSPECT)”

---

## 📌 Objective

To extract structured information from scanned handwritten medical prescriptions using Python, OCR (Tesseract), and rule-based logic to simulate a multimodal LLM.

---

## 🛠️ Tools and Libraries Used

- **Python 3**
- **Tesseract OCR** – Optical Character Recognition engine
- **OpenCV** – Open Source Computer Vision Library
- **pytesseract** – Python wrapper for Tesseract
- **pandas** – Data structuring and CSV export
- **json** – For saving structured data
- **os** – File handling

---

## 📂 Dataset

- **Name**: Handwritten Medical Prescription Images Dataset  
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/mehaksingal/illegible-medical-prescription-images-dataset)  
- **Description**: 129 scanned handwritten prescriptions in `.jpg` format

---

## ⚙️ Approach / Pipeline

### Step-by-Step Workflow:

1. **Preprocessing**  
   - Converted images to grayscale  
   - Applied median blurring and thresholding to improve text visibility

2. **Text Extraction**  
   - Used `pytesseract` to extract text from the images

3. **Rule-Based Structuring**  
   - Parsed OCR output line-by-line to extract:
     - Doctor Name
     - Patient Info
     - Age
     - Date
     - Medicines
     - Dosage
     - Signature

4. **Output**  
   - Stored the structured results in:
     - `structured_output.json`
     - `structured_data.csv`

---

## 💡 Sample Output

```json
{
  "filename": "63.jpg",
  "Doctor": "Dr A. Kumar",
  "Patient": "Rakesh",
  "Age": "42",
  "Date": "10-04-2025",
  "Medicines": ["Paracetamol 500mg", "Cetrizine 10mg"],
  "Dosage": ["1 tablet twice daily", "1 at night"],
  "Signature": "Dr A. Kumar"
}

How to Run This Project:
Installation
pip install opencv-python pytesseract pandas

Setup Tesseract (Mac)
import pytesseract
pytesseract.pytesseract.tesseract_cmd = "/opt/homebrew/bin/tesseract"

Run the notebook
jupyter notebook pipeline.ipynb

Folder Structure

ICMR_PROSPECT_Assignment/
├── prescriptions/                  # input images
├── output/
│   ├── json/
│   │   └── structured_output.json
│   └── structured_data.csv
├── pipeline.ipynb
├── ICMR_PROSPECT_Presentation.pptx
├── README.md

Deliverables
	•	✅ pipeline.ipynb – Jupyter Notebook with full code
	•	✅ structured_output.json – Extracted structured data
	•	✅ structured_data.csv – CSV version
	•	✅ ICMR_PROSPECT_Presentation.pptx – 3-slide summary presentation

Thank you for reviewing this assignment.
Please feel free to explore the code, data, and presentation shared in this repository.

— Barnita Das
