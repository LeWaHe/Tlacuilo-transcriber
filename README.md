Breakdown of the Tlacuilo transcriber folder and process:
- audio_files_drop : drop your audio file (mp3, WAV, m4a) here to have it converted to wav if needed and transcribed (typical delay on M1 chip: 1 min per 1 min audio). Once process starts a dummy file is created, its filename is used as a status to confirm processing and estimated run time. This status file is erased when transcription is completed.
- doc :  contains whisper_errors.xlsx where you may list common transcription errors in your domain and their corrections, these will be applied during transcription
- processed_audios : transcribed audio file is moved here
- scripts : contains the python script that automatically transcribes the audio
- transcripts : the transcript is saved here

Tlacuilo uses whisper locally, on the first run it will download the large-v2 model.

please note ffmpeg is requiered locally to convert audios
