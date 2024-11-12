# LLM-Powered Multimodal Voice Assistant

This project is a multimodal AI voice assistant that processes both audio and image inputs to generate descriptive text outputs and converts them to audio responses. The assistant is built using OpenAI's Whisper for speech recognition, Llava for image-to-text, and gTTS for text-to-speech functionality. This project also features a Gradio interface for user-friendly interactions.

## Features

- **Speech-to-Text**: Converts spoken audio input to text using OpenAI's Whisper model.
- **Image-to-Text**: Provides detailed descriptive analysis of uploaded images using the Llava model.
- **Text-to-Speech**: Converts the generated text responses back to audio using Google Text-to-Speech (gTTS).
- **Multimodal Interaction**: Supports both image and voice input, providing a flexible, interactive experience.
- **Gradio Interface**: Easy-to-use web interface for interacting with the assistant.

## Getting Started

### Prerequisites

- Python 3.10.9 or later
- GPU-enabled system (for better performance with Whisper and Llava models)
- [Gradio](https://gradio.app/), [Transformers](https://huggingface.co/docs/transformers/), and other required libraries

### Installation

Clone the repository and install the necessary libraries:
```bash
git clone <your-repo-url>
cd <your-repo-directory>



## Install dependencies:

pip install -q transformers==4.41.0
pip install bitsandbytes==0.41.3
pip install -q git+https://github.com/openai/whisper.git
pip install -q gradio
pip install -q gTTS


## Model Setup
Make sure you have access to the required models from Hugging Face:

Llava: llava-hf/llava-1.5-7b-hf
Whisper (OpenAI): Installed via whisper package

## Usage
Run the Application: Launch the assistant using the Gradio interface:

python <your-main-script>.py
Interact with the Assistant:

## Upload an image for visual analysis.
Use your microphone to provide a spoken prompt.
The assistant will return a detailed description of the image along with an audio response based on the image and audio inputs.


## Code Structure
img2txt: A function to process and describe the uploaded image using Llava.
transcribe: Uses Whisper to convert spoken audio input into text.
text_to_speech: Converts the generated text response into audio using gTTS.
process_inputs: Main function integrating image and audio processing.
Gradio Interface: Provides an interactive UI with options for image and voice input.

Example
After starting the interface, you will see options to upload an image, camera and record audio. The assistant will analyze the image and answer any relevant questions you ask through voice input.

## Requirements
transformers
bitsandbytes
whisper
gradio
gTTS
torch


## System Compatibility
This project requires Python 3.10.9. A CUDA-enabled GPU is recommended for optimal performance.

## Troubleshooting
Ensure all dependencies are installed as per the versions specified.
GPU support is required for faster inference; check torch.cuda.is_available() for CUDA availability.
Confirm that Llava, Whisper, and gTTS models are accessible and properly configured.


## Future Improvements
Add support for more advanced image question-answering.
Enable support for additional languages in speech-to-text and text-to-speech.
Optimize processing for real-time usage and mobile compatibility.


## Acknowledgments
OpenAI Whisper: For powerful speech-to-text capabilities.
Hugging Face: Providing model hosting and APIs for llava and other models.
Google Text-to-Speech (gTTS): For text-to-speech synthesis.


Screenshot:
