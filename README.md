# Voice Cloner: Multi-Language Audio Synthesis

## Overview
**Voice Cloner** is a project that uses a multilingual voice cloning model from Hugging Face to generate synthetic speech in the voice of a given audio sample. The project takes in an audio clip and a text input, and outputs a synthesized audio file with the cloned voice speaking the provided text.

The project utilizes **Hugging Face’s Voice-Clone-Multilingual** model to clone voices in multiple languages.

## Features
- **Voice Cloning**: Clone voices from short audio samples and synthesize text into the same voice.
- **Multilingual Support**: The model supports multiple languages for synthesis.
- **Easy Setup**: Ready-to-use functions to input your own audio and text.

## Project Structure

Voice-Cloner-Multilingual/
│
├── clone_voice.py # Contains all the code logic for voice cloning
├── input_audio.wav # Your input audio file (Example provided)
├── cloned_output.wav # The output file containing the cloned voice
├── README.md # Project description and usage instructions
└── requirements.txt # List of dependencies (torch, transformers, pydub)

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/RashidNoor42/Voice-Cloner-Multilingual.git
   cd Voice-Cloner-Multilingual
Install dependencies:
Create a virtual environment (optional but recommended):

python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Then install the dependencies:

pip install -r requirements.txt
Usage
Prepare your audio file:

Place a short audio clip that you want to clone (in .wav format) in the root directory of the project.

Prepare your text input:

Write the text that you want to clone the voice to speak.

Run the voice cloning function:

Open a Python environment or Jupyter notebook, and run the following code:

from clone_voice import clone_voice

# Specify the path to your audio file and the text you want to clone
audio_file = 'path_to_audio_clip.wav'
text = 'Hello, this is a cloned voice speaking.'

# Call the voice cloning function
output_audio = clone_voice(audio_file, text)
Listen to the cloned audio:
After running the code, you will find the output in a new file called cloned_output.wav which contains the cloned voice. You can also use this code to play the audio directly in Python:


import IPython.display as ipd

ipd.Audio(output_audio)
Requirements
Python 3.x

Libraries:

torch

transformers

soundfile

pydub

You can install all the dependencies at once by running:

pip install -r requirements.txt

**Model**
This project uses the Voice-Clone-Multilingual model hosted on Hugging Face. You can find more details on the model here:
Voice-Clone-Multilingual Model on Hugging Face

**Contributing
**Feel free to fork this project, make improvements, and submit pull requests. Any suggestions or improvements are welcome!

Author
Rashid Noor
https://github.com/rashidnoor42, https://www.linkedin.com/in/rashid-noor-b25962154/
---

### Key Sections:
1. **Overview**: Brief explanation of the project.
2. **Features**: Key functionalities of the project.
3. **Project Structure**: Breakdown of the directory structure.
4. **Setup Instructions**: Steps to clone and set up the project environment.
5. **Usage**: How to use the voice cloning functionality.
6. **Requirements**: Necessary libraries and dependencies.
7. **Model**: Info about the Hugging Face model used for voice cloning.
8. **License and Contributing**: Basic info on how to contribute.

Feel free to modify any parts of the `README.md` based on your preferences or specific project requirements!
