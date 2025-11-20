
🎬 Video Dubbing Automation System  
Automatic Video Translation & Dubbing into Indian Regional Languages

This project is an end-to-end automated pipeline that converts any English video into multiple Indian languages such as Hindi, Telugu, Tamil, Kannada, Malayalam, Bengali, and Marathi. It extracts the audio, separates vocals and background music, converts speech to text, translates the text, generates new speech in the target language, mixes audio, and finally reconstructs the video with the dubbed audio and optional subtitles.

Features:
- Convert MP4 → WAV
- Separate vocals and background music
- Speech-to-text using Google Speech Recognition
- Translate English text to any Indian language
- Text-to-speech for generating dubbed audio
- Adjust and equalize audio duration
- Merge translated audio with background music
- Extract video without sound
- Reattach merged audio to video
- Generate SRT subtitle files
- Add subtitles to video
- GUI for video compression (Tkinter)
- Uses FFmpeg, MoviePy, OpenCV, Spleeter, GoogleTrans, gTTS

Technologies Used:
Python 3, PyDub, FFmpeg, MoviePy, OpenCV, SpeechRecognition, GoogleTrans, gTTS, pysrt, Spleeter, Tkinter GUI

Installation:
pip install pydub ffmpeg-python moviepy SpeechRecognition googletrans==4.0.0-rc1 gtts pysrt opencv-python spleeter pygame

Workflow:
Input Video → Extract Audio → Separate Vocals → Speech-to-Text → Translate → Text-to-Speech → Adjust Duration → Mix Audio Tracks → Extract Video-Only → Merge with New Audio → Export Final Video → Generate SRT → Add Subtitles (Optional)

Folder Structure:
project/
│── README.txt
│── main.ipynb
│── audio/
│── video/
│── subtitles/
│── gui/

Step-By-Step Description:
1. Convert Video to Audio (MP4 → WAV)
2. Separate Music and Vocals using Spleeter
3. Convert Vocals to Text using SpeechRecognition
4. Translate Text to Target Indian Language
5. Convert Translated Text to Speech using gTTS
6. Sync Durations using padding
7. Merge Translated Audio + Music
8. Extract Video without audio
9. Merge new dubbed audio with video
10. Generate subtitles
11. Add subtitles to video (optional)

GUI Component:
A Tkinter GUI allows browsing videos, selecting codec (H264, H265, VP9, AV1, etc.), and compressing output.

Future Enhancements:
- AI voice cloning
- Lip sync automation
- Noise reduction using AI
- Cloud API version
- Multi-speaker support
