# freesound-kaggle

Hey! I'm pariticipating to the kaggle competition of free sound (https://www.kaggle.com/c/freesound-audio-tagging)

It's competition without prizes but just wanted to start without the pressure and try to apply the ML knowledge to
specific problems.

The way I'm working is with iterations, make something working and after each step think which is gonna to be 
my next iteration (wich thinks I'm gonna try)

### First step: MVP

This is the first attemp, on which basically the focus in:

- [ ] Loading the data
- [ ] Split train/validation
- [ ] Having the mapk metric (is how the LeaderBoard is calculated)
- [ ] Creating the result csv file

Basically I use two super simple features that librosa give you and use SVC from scikit-learn

### Second: SVM + MFCC

Just like the MVP but:

- [ ] Uses MFCC (from librosa)
- [ ] Does a search of the best parameters for SVM

### Third: CNN + MFCC

- [ ] ADD 3 CNN models (two with only 1D CNN and another with 2D CNN) 
- [ ] Since CNN needs a fixed size  (for the dense layer)
- [ ] Crop the MFCC to 5 seconds, if the audio is shorter, repeat until 5 seconds


### Fourth: CNN 5 seconds moving window

- [ ] Each clip is splitted in various 5 seconds split with a window that overlaps 1.5 seconds
- [ ] Also change the way the csv is computed


