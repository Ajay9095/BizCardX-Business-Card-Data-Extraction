# BizCardX: Business Card Data Extraction

## Overview
BizCardX is a Streamlit-based application that extracts and processes information from business cards using Optical Character Recognition (OCR) technology. It utilizes EasyOCR to extract text from images and provides options to modify, store, and delete extracted information using SQLite.

## Features
- Extracts text from business card images using EasyOCR
- Identifies and categorizes details such as Name, Designation, Company Name, Contact, Email, Website, Address, and Pincode
- Stores extracted details along with the original image in an SQLite database
- Provides an interactive Streamlit UI for previewing, modifying, and deleting records
- Supports uploading images in PNG, JPG, and JPEG formats

## Technologies Used
- Python
- Streamlit
- EasyOCR
- Pandas
- NumPy
- SQLite

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/bizcardx.git
   cd bizcardx
   ```
2. Install dependencies:
   ```bash
   pip install streamlit easyocr pandas numpy pillow sqlite3 streamlit-option-menu
   ```
3. Run the application:
   ```bash
   streamlit run app.py
   ```

## Usage
1. **Home Page:** Displays an introduction to the application.
2. **Upload & Modify:**
   - Upload a business card image
   - Extracts text and categorizes details
   - Saves the extracted details to an SQLite database
   - Allows previewing and modifying stored records
3. **Delete:**
   - Provides an option to delete records from the database

## Database Schema (`bizcardx.db`)
| Column       | Type    | Description                        |
|-------------|--------|------------------------------------|
| name        | TEXT   | Name of the person                |
| designation | TEXT   | Job designation                    |
| company_name| TEXT   | Company name                       |
| contact     | TEXT   | Contact number                     |
| email       | TEXT   | Email address                      |
| website     | TEXT   | Website URL                        |
| address     | TEXT   | Physical address                   |
| pincode     | TEXT   | Postal code                        |
| image       | BLOB   | Business card image (binary data)  |

## Contributing
If you’d like to contribute, please fork the repository and submit a pull request with improvements.

## License
This project is licensed under the MIT License.

## Contact
For any queries or support, please contact [your-email@example.com].

