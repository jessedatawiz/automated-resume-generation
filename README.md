# Automated Resume Generation

## Project Description
This project aims to help the job application process by automating the customization of curriculum vitae (CVs) for specific job descriptions. Manually tailoring a CV for each application is a time-consuming and often repetitive task. This solution leverages advanced natural language processing (NLP) and retrieval-augmented generation (RAG) techniques to dynamically generate optimized CVs, significantly streamlining the application workflow.

## Features
- **Intelligent CV Customization**: Automatically adapts your CV content based on the requirements of a new job description.
- **Personalized Data Integration**: Seamlessly retrieves and incorporates relevant information from your personal Google Drive folders (technical courses, certifications, professional experience, educational background).
- **Efficient Data Retrieval (RAG)**: Utilizes Chroma DB for robust and efficient retrieval of specific details from your stored documents.
- **Open-Source Model Power**: Built upon the powerful `CEIA-UFG/Gemma-3-Gaia-PT-BR-4b-it` open-source language model, ensuring high-quality text generation.
- **Free GPU Accessibility**: Designed to run efficiently on Google Colab's free GPU resources, making it accessible to a wide range of users.
- **Template-Based Output**: Generates a new PDF CV based on a user-provided template, maintaining your preferred formatting and style.
- **User-Friendly Workflow**: Simple input of a job description and a CV template to receive a tailored output.

## Technologies Used
- **Language Model**: `CEIA-UFG/Gemma-3-Gaia-PT-BR-4b-it` (Hugging Face)
- **Runtime Environment**: Google Colab (with free GPU access)
- **Vector Database**: Chroma DB
- **Data Storage**: Google Drive
- **Programming Language**: Python (and associated libraries for PDF generation, NLP, etc.)

## Setup
To set up and run this project, you will need:
- **Google Account**: For Google Colab and Google Drive access.
- **Hugging Face Account** (Optional but Recommended): To easily access the `Gemma-3-Gaia-PT-BR-4b-it` model.
- **Python Environment**: Although primarily run on Colab, local development might require Python 3.x.

### Detailed Setup Steps (to be elaborated):
1. Clone this repository.
2. Open the main Jupyter Notebook in Google Colab.
3. Grant necessary permissions for Google Drive access.
4. Install required Python libraries (e.g., `transformers`, `chromadb`, `pypdf`, `fpdf` or similar for PDF generation).
5. Structure your Google Drive folders as expected (e.g., `CV_Data/courses`, `CV_Data/experience`, `CV_Data/education`).
6. Upload your curriculum template (e.g., `my_template.pdf` or `my_template.tex`) to a designated folder.

## Usage
1. **Prepare Your Data**: Ensure your technical courses, certifications, professional experience, and educational information are well-documented within text files (e.g., `.txt`, `.md`, or `.docx`) in the specified Google Drive folders.
2. **Provide Your Template**: Have your custom curriculum template ready. This project will use it as the base for the generated PDF.
3. **Run the Colab Notebook**:
   - Execute the cells in the Google Colab notebook.
   - When prompted, input the new job description you wish to target.
   - The system will process your data, generate the customized content, and create a new PDF.
4. **Download Your New CV**: The generated PDF will be available for download from your Google Drive or directly from the Colab environment.

## Contributing
Contributions are welcome! Please feel free to open issues or submit pull requests.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
