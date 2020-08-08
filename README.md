# Speech-To-Text-in-python

Speech recognition has its roots in research done at Bell Labs in the early 1950s.
Early systems were limited to a single speaker and had limited vocabularies of about a dozen words.Modern speech recognition systems have come a long way since their ancient counterparts. They can recognize speech from multiple speakers and have enormous vocabularies in numerous languages.

# How Speech Recognition Works – An Overview

The first component of speech recognition is, of course, speech.

Speech must be converted from physical sound to an electrical signal with a microphone, and then to digital data with an analog-to-digital converter. 

Once digitized, several models can be used to transcribe the audio to text.



# Audio speech into text

Recognizing speech requires audio input, and SpeechRecognition makes retrieving this input really easy. Instead of having to build scripts for accessing microphones and processing audio files from scratch, SpeechRecognition will have you up and running in just a few minutes.

The SpeechRecognition library acts as a wrapper for several popular speech APIs and is thus extremely flexible. One of these—the Google Web Speech API—supports a default API key that is hard-coded into the SpeechRecognition library. 
              
Requirements:
       -->Python Speech Recognition module: pip install speechrecognition
       
       
Audio used: winston-churchill-the-threat-of-germany.wav
## Output

    Converting audio transcripts into text ...
    many people think that the best way to it take war in the development and println debate on the younger generation you are had the
       
# How about converting different audio language?

For example, if we want to read a french language audio file, then need to add language option in the recogonize_google. 

    #Adding french langauge option
    text = r.recognize_google(audio_text, language = "fr-FR")
    
# Microphone speech into text

We need to install PyAudio library which used to receive audio input and output through the microphone and speaker.
Basically, it helps to get our voice through the microphone.
    
Requirements:
       -->PyAudio:  pip install pyaudio
       
Instead of audio file source, we have to use the Microphone class. Remaining steps are the same.

I just talked "Hi,I'm Santhosh"

## Output

    Text: hi I am Santosh

# How about talking in a different language?
Again, we need to add the required language option in the recognize_google(). 
For Example Tamil, Indian language and add “ta-IN” in the language option.

    #Adding "tamil language"
    print(“Text: “+r.recognize_google(audio_text, language = “ta-IN”))

# Note

Google speech recognition API is an easy method to convert speech into text, but it requires an internet connection to operate.
