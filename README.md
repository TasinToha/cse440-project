# CSE440 AI Project: Rock Paper Scissors Game

This project is part of **CSE440: Artificial Intelligence** and showcases a Rock Paper Scissors game where a user plays against an AI. The AI uses deep learning to recognize hand gestures in real time.

---

## Features  
- **Gesture Recognition**: Detects hand gestures (rock, paper, scissors) via webcam.  
- **AI Model**: Uses a lightweight CNN model called **SqueezeNet** for accurate recognition.  
- **Real-Time Gameplay**: Recognizes user moves instantly and determines the winner.  
- **Interactive Experience**: Provides immediate feedback on each round.  

---

## How It Works  

1. **Image Collection**: Capture hand gesture images ("rock," "paper," "scissors," and "none") using a webcam.  
2. **AI Model Training**: Train a SqueezeNet model to classify gestures into four categories.  
3. **Game Logic**: The AI compares the user’s gesture with its own random move and decides the winner.  


---


## Requirements
- Python 3.7
- Keras
- Tensorflow
- OpenCV


---


## Steps to Run  

1. **Install Required Packages**:  

```sh
$ pip install -r requirements.txt
```

2. **Gather Images for each gesture**

```sh
$ python3 gather_images.py rock 500
```

3. **Train the model**

```sh
$ python3 train.py
```

4. **Test the model on some images**

```sh
$ python3 test.py <path_of_test_image>
```

5. **Play the game with your computer**

```sh
$ python3 play.py
```