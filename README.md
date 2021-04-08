# Real time feedback for words you flag as "bad"

### Steps
1. Clone repo
2. Followed setup tutorial [here](https://www.youtube.com/watch?v=Itic1lFc4Gg&t=1s&ab_channel=yingshaoxo%27slab) to download your model (save it in the directory and name it "model"). Note I'm using the [alphacephei api](https://alphacephei.com/vosk/install). 
3. Edit the bad words in run.py
4. Run run.py

The reason for choosing this api is because it can process words in realtime (offline). To be able to get feedback on your presentation/zoom call, offline speech recognition is required. Other packages like [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) are too slow and don't categorize "um" as a word. 

### Potential Next Steps
1. Make the i'm vs. um distinction more robust
2. Add feedback on tone shift
3. Provide post talk summary of your presentation (most/least frequent words, total time not speaking, etc.)

Any ideas/modifications/comments are welcome.
