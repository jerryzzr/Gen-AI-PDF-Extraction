# Creditsafe Gen AI Engineer - Text Information Extraction with OpenAI API

This Jupyter Notebook demonstrates the process of extracting key pieces of information from text files using OpenAI's GPT-4 API. The notebook provides an interactive interface to upload and process text files, clean the data, and extract structured information in JSON format.

## Features

### 1. **OCR for Text Extraction**  
   - Utilizes tools like [Umi-OCR](https://github.com/hiroi-sora/Umi-OCR) to extract text from PDF files.  
   - The OCR tool is ideal for documents that are in image or scanned formats.

### 2. **Text Preprocessing**  
   - **Google Translation Integration**: Translates non-English text into English for better processing and understanding.  
   - **SpaCy Text Cleaning**: Utilizes the SpaCy library to clean the text by removing unwanted characters, fixing spacing, and normalizing the content.  
   - Outputs preprocessed content as text files for further processing.

### 3. **Information Extraction Using OpenAI API**  
   - **Extract Key Information**: Uses the OpenAI GPT-4 API to extract specific information such as:
     - **Company Name**
     - **Company Identifier**
     - **Document Purpose**
   - The model is fine-tuned for advanced text understanding to accurately extract relevant details.

### 4. **Interactive Interface**  
   - **File Upload**: Provides an easy-to-use interface to upload files for processing.
   - **Folder Selection**: Allows users to select input and output folders, ensuring smooth data management.

### 5. **JSON Output**  
   - After extracting the key information, the notebook generates a structured JSON output that can be easily consumed by other applications or systems.
## Folder Structure Explanation
1. **original files**: This folder contains the original PDF files to be processed.
2. **text extract**: In this folder, you'll find the text extracted from the PDF files in their raw form.
3. **translated**: This folder holds the translated text files, where the content has been converted into the desired language.
4. **cleaned**: Here, you'll find the text files that have undergone preprocessing, including text cleaning and formatting adjustments.
5. **json_output**: This is where the final output is stored, containing the structured information (Company Name, Company Identifier, and Document Purpose) in JSON format.
## Workflow

1. **Upload Input Files**: Upload text or OCR-extracted text files for processing.
2. **Text Preprocessing**: The notebook cleans and normalizes the text, including translation and SpaCy text cleaning.
3. **Data Extraction**: OpenAI’s GPT-4 API extracts the following key data from the cleaned text:
   - Company Name
   - Company Identifier
   - Document Purpose (e.g., contract, resignation)
4. **Export as JSON**: The extracted information is saved in a structured JSON format, making it ready for further use or analysis.

## Installation Requirements

To run this notebook, make sure you have the following dependencies installed:

- **Python 3.x**
- **OpenAI API Key**: You will need an API key to access OpenAI services.
- **Required Libraries**:
  - `openai`
  - `spacy`
  - `tkinter`
  - `googletrans`
  - Other libraries as listed in `requirements.txt`

