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

## Project Structure

```plaintext
.
├── images/                         # Dataset of hand gestures
│   ├── rock/                       # Images of "rock" gestures
│   ├── paper/                      # Images of "paper" gestures
│   ├── scissors/                   # Images of "scissors" gestures
│   └── none/                       # Images with no hand gesture
├── gather_images.py                # Script to capture hand gesture images
├── train.py                        # Script to train the SqueezeNet model
├── test.py                         # Script to test the model and debug predictions
├── play.py                         # Script to play Rock Paper Scissors with the AI
├── rock-paper-scissors-model.h5    # Trained model file
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation

## Requirements
- Python 3.7

Secondly, Install the dependencies

```sh
$ pip install -r requirements.txt
```
