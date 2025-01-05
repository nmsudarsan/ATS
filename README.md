
# ATS Resume Expert

ATS Resume Expert is a Streamlit application designed to analyze resumes and job descriptions, leveraging Google Generative AI (Gemini) to evaluate and provide insightful feedback. The tool helps candidates improve their resumes to align better with job descriptions.

## Features

- **Resume Evaluation**: Provides professional feedback on how well a resume aligns with the provided job description.
- **Percentage Match**: Calculates the percentage match between a resume and the job description, highlighting missing keywords and providing actionable insights.
- **PDF Support**: Accepts resumes in PDF format and extracts content for analysis.

## Tech Stack

- **Python**: Core programming language.
- **Streamlit**: Web application framework.
- **Google Generative AI**: Used for generating intelligent feedback and match percentages.
- **pdf2image**: Converts PDF files to images for processing.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/ats-resume-expert.git
   cd ats-resume-expert
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Install Poppler (required by `pdf2image` for PDF processing):

   - **Windows**: Download and install Poppler from [Poppler for Windows](http://blog.alivate.com.au/poppler-windows/). Add the `bin` folder to your system's PATH.
   - **macOS**: Install via Homebrew:
     ```bash
     brew install poppler
     ```
   - **Linux**: Install using the package manager:
     ```bash
     sudo apt-get install poppler-utils
     ```

4. Create a `.env` file in the project directory and add your Google API key:

   ```env
   GOOGLE_API_KEY="your-google-api-key"
   ```

## Usage

1. Run the application:

   ```bash
   streamlit run app.py
   ```

2. Open the application in your browser at `http://localhost:8501`.

3. Upload your resume (PDF format) and enter the job description.

4. Click on the buttons to get feedback or percentage match.

## File Structure

```
.
├── app.py              # Main application file
├── requirements.txt    # Python dependencies
├── .env                # Environment variables (not included in version control)
└── README.md           # Project documentation
```

## Requirements

- Python 3.8 or higher
- Dependencies listed in `requirements.txt`

## Troubleshooting

- **Poppler Not Found**: Ensure Poppler is installed and its path is added to the system's PATH environment variable.
- **Google API Key Issues**: Check if the API key in `.env` is correct and has sufficient permissions.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## Author

Sudarsan

---

Happy coding! 🎉
