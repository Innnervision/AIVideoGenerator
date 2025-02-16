﻿# AIVideoGenerator

# Text to Animated Video Generator

This project is a GUI application built with Tkinter that generates animated videos from text input. The application uses the Stable Diffusion model to generate images and animates them using MoviePy. Additionally, Google Cloud Text-to-Speech is used to generate audio narration from the text input. 

## Features

- Converts text input into animated videos with zoom-in effects.
- Uses the Stable Diffusion model to generate images based on text prompts.
- Utilizes Google Cloud Text-to-Speech to generate narration for the video.
- Simple and intuitive GUI built with Tkinter.
- Allows saving the generated video to a file.

## Requirements

- Python 3.6 or higher
- Tkinter
- PIL (Pillow)
- MoviePy
- NumPy
- Torch
- diffusers (Stable Diffusion)
- Google Cloud Text-to-Speech
- spaCy

## Installation

1. **Clone the repository**

    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Set up a virtual environment**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies**

    ```bash
    pip install -r requirements.txt
    ```

4. **Download spaCy model**

    ```bash
    python -m spacy download en_core_web_sm
    ```

5. **Set up Google Cloud Text-to-Speech**

    - Create a Google Cloud project and enable the Text-to-Speech API.
    - Create a service account key and download the JSON file.
    - Set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable to the path of the JSON key file.

    ```bash
    export GOOGLE_APPLICATION_CREDENTIALS="path/to/your/google-cloud-key.json"
    ```

    On Windows:

    ```cmd
    set GOOGLE_APPLICATION_CREDENTIALS=path\to\your\google-cloud-key.json
    ```

## Usage

1. **Run the application**

    ```bash
    python VideoGenerator.py
    ```

2. **Enter text**

    - Type or paste the text into the text entry widget.

3. **Generate video**

    - Click the "Generate Video" button to start the process.
    - The application will generate images, animate them, and combine them into a video with narration.
    - The video will be automatically played once it's generated.
    - You will be prompted to save the video if desired.

## File Structure

- `VideoGenerator.py`: The main script containing the application logic.
- `requirements.txt`: List of dependencies.
- `README.md`: This readme file.

## Contributing

1. **Fork the repository**
2. **Create a new branch**

    ```bash
    git checkout -b feature/your-feature-name
    ```

3. **Make your changes**
4. **Commit your changes**

    ```bash
    git commit -m "Add some feature"
    ```

5. **Push to the branch**

    ```bash
    git push origin feature/your-feature-name
    ```

6. **Open a pull request**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Stable Diffusion](https://github.com/CompVis/stable-diffusion) for image generation.
- [Google Cloud Text-to-Speech](https://cloud.google.com/text-to-speech) for generating audio narration.
- [MoviePy](https://zulko.github.io/moviepy/) for video creation and manipulation.
- [spaCy](https://spacy.io/) for natural language processing.

