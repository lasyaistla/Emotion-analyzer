How to Use
1. Upload Your Video
Upload your video file. Supported formats include .mp4, .mov, .avi, etc.

2. Run the Script
Once you’ve uploaded the video, run the provided Python script. The following steps will occur:

Audio Extraction: The audio will be extracted from the video.
Speech-to-Text: The audio will be transcribed to text using Whisper.
Emotion Detection: The transcribed text will be analyzed to detect the emotion using DistilRoBERTa.
Subtitles: Subtitles will be generated and displayed on the video.
3. Results
After running the script, the following will be displayed:

Transcribed Text: The transcription of the audio.
Detected Emotion: The emotion detected from the transcription.
Confidence: The confidence score (between 0 and 1) of the emotion detected.
Pie Chart: A pie chart illustrating the confidence of the detected emotion.
Script Breakdown
1. Audio Extraction
The extract_audio_from_video() function extracts audio from the video using pydub.

2. Speech-to-Text
The transcribe_audio_to_text() function uses Whisper for automatic transcription of audio to text.

3. Emotion Detection
The detect_emotion() function uses Hugging Face’s DistilRoBERTa model to analyze the text and detect emotions.

4. Subtitles Generation
The create_subtitles() function generates subtitles and overlays them on the video. It splits the transcribed text into manageable chunks and displays them as subtitles on the video.

5. Visualization
The visualize_emotion() function generates a pie chart showing the detected emotion and its confidence score using matplotlib.![image](https://github.com/user-attachments/assets/b53725a2-8aef-4427-b71a-907f191a0836)

