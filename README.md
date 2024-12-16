# Sithafal_Task1

#### Simple Workflow for Task 1
1. Input PDF Upload:
The user uploads a PDF document (e.g., `sample.pdf`).
2. Data Extraction:
Text Extraction:
• Extract text directly using `pdfplumber` for text-based PDFs.
• For image-based or empty-text pages, perform OCR using `pytesseract`.
Table Extraction:
• Use `pdfplumber` to identify and extract tables.
• Clean the extracted tables for better alignment.
3. Text Preprocessing:
Normalize the extracted text to remove:
• Extra spaces, line breaks, and unwanted characters.
• Non-ASCII characters.
• Ensure consistent formatting.
4. Dynamic Formatting:
Parse and dynamically format the data:
• Extract degrees (e.g., Doctoral, Master's) and align with their corresponding percentages or 
monetary values.
Present the cleaned text line by line.
5. Output Generation:
Text Output: Display formatted textual data for the requested page(s).
Tabular Output: Show the extracted table as a structured DataFrame.

Technologies and Modules Used
# Technologies:
1. PDF Parsing and OCR:
Extract text from PDFs with both text-based and image-based pages.
Preprocess images for better OCR accuracy.
2. Data Preprocessing:
Normalize and clean data for structured output.
3. Dynamic Formatting:
Use regex patterns to dynamically parse and align data.
4. Tabular Processing:
Extract, clean, and display tables using Python libraries.



# Python Modules:
1. `pdfplumber`:
Extracts text and tables from PDF files.
2. `pytesseract`:
Performs OCR for image-based PDF pages.
3. `Pillow (PIL)`:
Enhances images (grayscale conversion, resizing, contrast) for better OCR.
4. `pandas`:
Formats tabular data into structured DataFrames.
5. `re`:
Dynamically parses text with regular expressions.

## Simplified Workflow Visualization
1. Upload PDF 
 ↓ 
2. Extract Data 
Text: Use `pdfplumber` or OCR (`pytesseract`). 
Tables: Extract with `pdfplumber`. 
 ↓ 
3. Preprocess Data 
Clean text and normalize tables. 
 ↓ 
4. Format Output 
Text: Align degrees with values dynamically. 
Tables: Display clean DataFrame. 
 ↓ 
5. Display Results 
This workflow ensures accurate extraction, preprocessing, and structured display of both textual and 
tabular data
