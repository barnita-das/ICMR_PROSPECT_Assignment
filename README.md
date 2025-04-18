### ICMR PROSPECT Phase-1 Screening Assignment

### Submitted by: Barnita Das

This project is a part of the screening assignment for the post of Project Research Scientist-I at PGIMER Chandigarh, under the project titled:

“An endoscopic ultrasound image-based Prediction and Risk Observation System for chronic Pancreatitis Evaluation using Convolutional Neural Network Technique (PROSPECT)”

### Objective

The goal is to extract useful and structured information from handwritten medical prescriptions, using Python and a simulated multimodal approach.

### Tools & Libraries Used

- Python 3
- OpenCV
- pytesseract (OCR)
- pandas
- Jupyter Notebook

### Dataset

- Total files: 129 scanned prescription images (`.jpg`)
- Source: Kaggle Handwritten Medical Prescription Dataset  
  (URL: [Click here](https://www.kaggle.com/datasets/mehaksingal/illegible-medical-prescription-images-dataset))

### Approach / Pipeline

1. Read and preprocess each image (convert to grayscale, remove noise).
2. Use Tesseract OCR to extract text from the image.
3. Apply simple rules to identify fields like:
   - Doctor Name
   - Patient Name
   - Age
   - Date
   - Medicines
   - Dosage
4. Save the final structured data into:
   - `structured_output.json`
   - `structured_data.csv`

This simulates how a multimodal LLM would extract structured information from an image + text input.

### Results

- Total images processed: 129
- Successfully extracted: 108
- Skipped: 21 (due to poor image quality or no text detected)

### Project Files

ICMR_PROSPECT_Assignment/
├── prescriptions/                  
├── output/
│   ├── json/
│   │   └── structured_output.json
│   └── structured_data.csv
├── pipeline.ipynb                 
├── ICMR_PROSPECT_Presentation.pptx
├── README.md

### Deliverables

- `pipeline.ipynb`: Code for the full pipeline
- `structured_output.json`: JSON file with extracted info
- `structured_data.csv`: CSV version of the output
- `ICMR_PROSPECT_Presentation.pptx`: PowerPoint (3-slide summary)

Thank you for the opportunity.  
Feel free to review the code and files shared here.

— Barnita Das
