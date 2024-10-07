# OCR Speech-to-Text Summarizer & Question Generator  

This project is a comprehensive tool that integrates Optical Character Recognition (OCR), Speech-to-Text capabilities, text summarization, and question generation. Utilizing Llama 3.2 with 1B parameters for summarization and question generation, the tool accepts text input from various formats including PDFs, PowerPoint presentations, Word documents, images, and audio files. Users can summarize text, generate questions, or perform both functions. The application will default to text extraction only if no options are selected. 

![ocr-speech-to-text](https://github.com/user-attachments/assets/ded03f4f-748a-44fb-8aad-0795f297c4db)


## Table of Contents  

- [Features](#features)  
- [Prerequisites](#prerequisites)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Model and Libraries](#model-and-libraries)  
- [Interface](#interface)  
- [Contributing](#contributing)  
- [License](#license)  
- [Acknowledgements](#acknowledgements)  

## Features  

- **Text Extraction**: Extract text from various sources including PDFs, Word documents, PowerPoint files, images, and audio recordings.  
- **Speech Recognition**: Convert speech from audio files to text using speech recognition libraries.  
- **Summarization**: Summarize extracted text using the Llama 3.2 model, allowing users to specify the number of summary words.  
- **Question Generation**: Generate questions with their answers based on extracted or summarized text, with the option to specify the number of questions.  
- **User Interface**: A Gradio-based interface for easy interaction and testing.  

## Prerequisites  

Ensure you have the following installed on your machine:  

- **Python 3.7 or higher**  
- **System Dependencies**:  
  - Install Tesseract OCR:  

    ```bash  
    sudo apt-get install tesseract-ocr -y  
    sudo apt-get install tesseract-ocr-ara -y  
    ```  

- A GPU is recommended for optimal performance.

## Installation  

1. Clone the repository:  

   ```bash  
   git clone https://github.com/OmaR099/OCR-Speech-To-Text-Summarizer-QuestionGenerator.git  
   cd OCR-Speech-To-Text-Summarizer-QuestionGenerator
   ```
   
2. Install the required libraries:

- **Python Libraries**: You can install the necessary Python libraries using the `requirements.txt` file included in this repository:  

    ```bash  
    pip install -r requirements.txt  
    ```

## Usage

1. Text Extraction: You can input text through files (PDF, PowerPoint, Word, images) or audio recordings. The tool supports both English and Arabic languages.

2. Choose Functionality:

You can select whether to summarize the text, generate questions, or both.
Specify the number of words for the summary and the number of questions to generate.
If none are selected, the tool defaults to extracting the text only.

## Model and Libraries

This project utilizes the following libraries and models:

- OCR: Implemented using PyTesseract for text extraction from images and documents.
- Speech-to-Text: Utilizes the following libraries:
    - speech_recognition
    - pydub
- Summarization and QG: Powered by Llama 3.2 1B model.

<img src="https://github.com/user-attachments/assets/941528d9-0d16-45ce-ab8d-5d346efa2a60" alt="image" width="330" height="330" />
<img src="https://github.com/user-attachments/assets/d0a7db6b-ed70-4c2d-b822-4b234e4c65f1" alt="image" width="330" height="330" />

## Interface

The project includes a Gradio interface for user interaction. Once the application is running, open the interface in a web browser to start extracting text, summarizing, or generating questions.

**Audio**

![audio](https://github.com/user-attachments/assets/b0fcd0b6-b942-4396-8471-6792537aff8d)

![audio2](https://github.com/user-attachments/assets/209eaf68-b4d2-442b-860f-ee52e919e3de)


**OCR & Documents**

![OCR](https://github.com/user-attachments/assets/525be5c3-1c12-423b-8071-803a9f1accbc)

![Screenshot 2024-10-07 220105](https://github.com/user-attachments/assets/3193787d-7ad9-445a-94b3-ede49d1de1e6)

![image](https://github.com/user-attachments/assets/18abcec8-e719-43ca-ae59-bece69fbaf4d)

## Contributing

Contributions are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Commit your changes (git commit -m 'Add new feature').
4. Push to the branch (git push origin feature-branch).
5. Open a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgements

- Llama and its creators for providing powerful language models.
- PyTesseract for effective OCR capabilities.
- SpeechRecognition and Pydub for their contributions to speech-to-text conversions.
- Gradio for providing an excellent interface for testing and interaction.
- Contributors and the open-source community for guidance and support.
