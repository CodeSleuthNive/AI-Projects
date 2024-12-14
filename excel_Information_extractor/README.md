# Excel Sheet Query Tool

## Overview
The **Excel Sheet Query Tool** is a Streamlit-based web application that allows users to upload an Excel file, explore its data, and ask AI-powered questions about the data using the Google Gemini API. This tool is designed to simplify data analysis by leveraging AI to extract insights from spreadsheet data.

---

## Features

- **Excel File Upload**: Upload `.xlsx` files and view their sheet names.
- **Sheet Selection**: Select a specific sheet to analyze.
- **Data Preview**: Display the content of the selected sheet in a tabular format.
- **AI-Powered Queries**: Use natural language to ask questions about the uploaded data.
- **Google Gemini Integration**: Utilize the Google Gemini API for generating intelligent responses.

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/excel-sheet-query-tool.git
   cd excel-sheet-query-tool
   ```

2. **Set Up Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure Environment Variables**
   - Create a `.env` file in the project root directory.
   - Add your Google Gemini API key to the `.env` file:
     ```env
     GEMINI_API_KEY=your_google_gemini_api_key
     ```

5. **Run the Application**
   ```bash
   streamlit run app.py
   ```

---

## Usage

1. Open the web application in your browser (usually `http://localhost:8501`).
2. Upload an Excel file (`.xlsx`).
3. Select a sheet from the uploaded file to analyze.
4. Preview the data of the selected sheet.
5. Type your question about the data in the input box.
6. Click the **Ask AI** button to receive an AI-generated response.

---

## File Structure

```plaintext
excel-sheet-query-tool/
├── app.py                  # Main application script
├── config.py               # Configuration file for sensitive keys
├── requirements.txt        # List of Python dependencies
├── .env                    # Environment variables (ignored by Git)
└── README.md               # Project documentation
```

---

## Dependencies

- **Streamlit**: For building the web interface.
- **Pandas**: For handling Excel data.
- **Google Generative AI (gemini)**: For AI-powered responses.
- **dotenv**: For managing environment variables.

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## Environment Variables

The application requires a valid API key for the Google Gemini API. Ensure you set up the `.env` file as shown:

```env
GEMINI_API_KEY=your_google_gemini_api_key
```

The `GEMINI_API_KEY` is essential for connecting to the Google Gemini service.

---

## Troubleshooting

1. **Missing API Key**
   - Ensure the `.env` file is properly configured.
   - Check if the `dotenv` library is installed.

2. **Error Reading Excel Files**
   - Verify that the uploaded file is a valid `.xlsx` file.
   - Ensure the file is not corrupted.

3. **AI Response Errors**
   - Confirm that the Google Gemini API is accessible and your API key is valid.
   - Check the `generation_config` parameters for compatibility with your model version.

---

## Future Enhancements

- Add support for other file formats (e.g., `.csv`, `.xls`).
- Enable advanced filtering and sorting of data.
- Provide visualizations (charts, graphs) for better insights.
- Improve error handling and user feedback.

---

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and submit a pull request. Make sure to include detailed documentation of your changes.

---


## Acknowledgments

- [Streamlit](https://streamlit.io/) for the amazing framework.
- [Google Gemini](https://ai.google/) for AI-powered data insights.
- Open-source community for inspiration and resources.

