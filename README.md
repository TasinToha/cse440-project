# cse440-project

# Rock Paper Scissors Game

This project is developed as part of **CSE440: Artificial Intelligence** and implements a Rock Paper Scissors game where the user can play against an AI. The AI detects and recognizes the user's hand gesture using deep learning with a convolutional neural network called **SqueezeNet**.

## Features
- **Hand Gesture Detection**: The game captures the user's move (rock, paper, or scissors) using a webcam.
- **Deep Learning Model**: The AI model is built using SqueezeNet, a lightweight and efficient CNN.
- **Real-Time Prediction**: The user's move is recognized in real-time and compared against the AI's randomly generated move.
- **Interactive Gameplay**: Provides feedback to the user about the winner of each round.

---

## How It Works

1. **Data Collection**:
   - Hand gesture images for "rock," "paper," "scissors," and "none" are captured using a webcam.
   - Collected images are stored in the `images/` directory, organized by class labels.

2. **Model Training**:
   - A SqueezeNet-based CNN model is trained on the collected images.
   - The model classifies the user's hand gesture into one of four categories: "rock," "paper," "scissors," or "none."
   - Training is implemented in `train.py`.

3. **Game Logic**:
   - The game compares the user's move (detected by the model) with the AI's random move.
   - Displays the winner of each round.


---


## Requirements
- Python 3.7
- Keras
- Tensorflow
- OpenCV

Install the dependencies

```sh
$ pip install -r requirements.txt
```

Gather Images for each gesture
```sh
$ python3 gather_images.py rock 500
```

4. Train the model
```sh
$ python3 train.py
```

5. Test the model on some images
```sh
$ python3 test.py <path_of_test_image>
```

6. Play the game with your computer
```sh
$ python3 play.py
```