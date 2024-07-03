## Audio to SOAP Note Generation

### Project Overview

This project provides a Flask-based web service that converts audio files into SOAP (Subjective, Objective, Assessment, Plan) notes. The service uses Whisper for transcription and Ollama for generating the SOAP notes.

### Features

- **Transcription**: Converts audio files to text using Whisper.
- **SOAP Note Generation**: Creates SOAP notes from transcribed text using Ollama.
- **API Endpoints**: 
  - `/transcribe`: For transcribing audio files.
  - `/generate_soap`: For generating SOAP notes from the transcribed text.

### Project Structure

- `main.py`: Main application file containing the Flask web service and logic for transcription and SOAP note generation.

### Dependencies

- Python 3.10
- Flask
- Whisper
- LangChain Community (Ollama) #install ollama llama3 locally on your system

### Installation

1. **Clone the repository**
   ```sh
   git clone https://github.com/yourusername/audio-to-soapnote-generation.git
   cd audio-to-soapnote-generation
   ```

2. **Create a virtual environment and activate it**
   ```sh
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages**
   ```sh
   pip install -r requirements.txt
   ```

4. **Ensure Whisper and Ollama models are correctly set up**

### Running the Application

To run the Flask application, execute the following command:
```sh
python main.py
```
The application will start in debug mode and listen on `http://127.0.0.1:5000/`.

### API Endpoints

#### `/transcribe`
**Method**: `POST`

**Description**: Transcribes audio files to text.

#### `/generate_soap`
**Method**: `POST`

**Description**: Generates SOAP notes from transcribed text.


### Acknowledgments

- Whisper for transcription
- LangChain Community (Ollama) for SOAP note generation


