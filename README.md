# Semnatic Time series transcription approach with open source available models

The practice project to explore open source models and their performance for english language transcriptions on any given video.
This repository contains Code for the time series semantic chunking of audio extracted from a [youtube video]( https://youtu.be/Sby1uJ_NFIY?si=QCGzzQptwQgW78o9) and A simple gradio interface to perform this purpose and return time series transcription of any given youtube link.

The open source model tested to perform this task is OpenAI's whisper -s. [Link](https://github.com/openai/whisper)

**Possible Generalizations, Limitations and Adoptation stratigies**

As tested in some of the scenarios, this approach can be used in scenarios like transcriptions of dubbed movies and anime even while using the whisper 'base' model. It can prove efficient to transcribe large audio files given that the audio is clean with minimal background noice.  
There are few limitation of base model which can be solved by higher Whisper models. eg- it can only process English language. Also it was observed when the model was given a song to transcribe, even when the pronaunciations of the lyrics were clear due to music in the background the transcription quality was observed to go down significantly.
This problems can be solved with Whisper 'large' model as it takes in account large amount of parameters, voice activity detection is one of the speech processing task Whisper is trained on so it is more robust to musical interuptions, It is also inbuilt with spoken language identification and speech translation widens the domain of applications of this approach which includes Multilingual transcription and translation.

If computational time is concern other approach is with noice removal/cleaning the audio file, seperating speech from music element before processing the audio which an also yeild better results.
As it's a prove method which yeild better results when training and testing data on audio classification tasks.
