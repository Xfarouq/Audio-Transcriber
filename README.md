# Audio Transcription App

This project provides a simple interface for transcribing audio files into text using OpenAI's Whisper model. It uses **PyTorch**, **Transformers**, and **Gradio** to process audio and provide real-time transcription.

---

## Features

- **Automatic Speech Recognition (ASR):** Utilizes the OpenAI Whisper `tiny.en` model for transcription.
- **User-friendly interface:** Powered by Gradio for easy audio upload and text output.
- **Efficient processing:** Processes audio files in 30-second chunks for faster results.

---

## How It Works

1. **Upload an audio file:** The app accepts audio files in various formats through the Gradio interface.
2. **Transcription:** The audio file is processed using the Whisper model to generate the transcribed text.
3. **Output:** The transcribed text is displayed in a textbox for the user to copy or review.

---

## Requirements

Make sure to have the following Python packages installed:

- `torch`
- `transformers`
- `gradio`

Install them using:

```bash
pip install torch transformers gradio
```

---

## Usage

1. Clone this repository or copy the script into your project.
2. Save the code in a Python file, e.g., `audio_transcription_app.py`.
3. Run the script:

   ```bash
   python audio_transcription_app.py
   ```

4. Open the Gradio app in your browser (a link will be displayed in the terminal).
5. Upload an audio file and view the transcribed text.

---

## Code Overview

- **`transcript_audio(audio_file):`**  
  Function that processes the uploaded audio file using the Whisper model for transcription.

- **Gradio Interface:**  
  - **Input:** `gr.Audio` allows users to upload audio files.
  - **Output:** `gr.Textbox` displays the transcription result.

---

## Future Enhancements

- Support for multilingual transcription.
- Add support for real-time audio recording.
- Improve the UI with additional customization options.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

### Acknowledgements

- **Hugging Face Transformers:** For providing the Whisper model integration.
- **Gradio:** For the simple and powerful interface design.
