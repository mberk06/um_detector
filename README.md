# Real time feedback for words you flag as "bad"

![check /example.gif]("example.gif")


### Steps
1. Clone repo
2. Download the [speech recognition model](https://alphacephei.com/vosk/models) and save to `um_detector` directory (rename model download as "model"): Here's a [setup tutorial](https://www.youtube.com/watch?v=Itic1lFc4Gg&t=1s&ab_channel=yingshaoxo%27slab) and the model's [alphacephei api](https://alphacephei.com/vosk/install). 
3. Edit the bad words in run.py (or leave as is)
4. Run `pip install vosk; pip install sounddevice` in terminal
5. Run run.py

The reason for choosing this api is because it can process words in realtime (offline). To be able to get feedback on your presentation/zoom call, offline speech recognition is required. Other packages like [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) are too slow and don't categorize "um" as a word. 

### Potential Next Steps
1. Make the i'm vs. um distinction more robust
2. Add feedback on tone shift
3. Provide post talk summary of your presentation (most/least frequent words, total time not speaking, etc.)

Any ideas/modifications/comments are welcome.

