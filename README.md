# Emotion-Detection-Using-Cv2-and-FER-
Key Sections of the Code
Importing Required Libraries:
IPython.display: Used to display JavaScript in the Colab notebook.
google.colab.output: Allows evaluation of JavaScript code to capture the photo.
base64: For decoding the image data captured from the webcam.
numpy: A library for numerical operations (not extensively used here).
cv2 (OpenCV): For image processing.
PIL: For opening and displaying images.
random: For random selections in games.
FER: The emotion detection library.
# Function to Capture Image from Webcam:
This function displays a button to capture a photo using the user's webcam.
The captured image is processed and saved to a file named photo.jpg.
# Emotion Detection Function:
Reads the captured image using OpenCV.
Uses the FER detector to analyze the image for emotions.
Identifies the dominant emotion based on the highest score and returns it.
# Game Functionality Based on Detected Emotion:
This function determines which game to play based on the detected emotion:
Happy: Rock-Paper-Scissors
Sad: Snakes and Ladders
Angry: Tic-Tac-Toe
Fear: Riddles
Surprise: Guess the Number
Neutral: Scrambled Words
Individual Game Functions:

# Rock-Paper-Scissors:
def rock_paper_scissors():
    ...
# Snakes and Ladders:
def snakes_and_ladders():
    ...
# Tic-Tac-Toe:
python
# def tic_tac_toe():
    ...
# Guess the Number:
def guess_the_number():
    ...
# Scrambled Words:
def scrambled_words_multiple():
    ...
Riddles:
def riddles():
    ...
Each of these functions implements the logic for the respective games. They interact with the user via console input, checking for valid moves and determining game outcomes.
# Winner Check Function:
def check_winner(board, player):
    ...
This function checks if a player has won the Tic-Tac-Toe game by evaluating winning combinations.
# Main Program Flow:
filename = take_photo()
detected_emotion = detect_emotion(filename)
play_game_based_on_emotion(detected_emotion)
The main sequence of the program where:
An image is captured.
Emotion is detected from the image.
A game is initiated based on the detected emotion.
# Summary
The program utilizes a combination of JavaScript for webcam access, OpenCV for image processing, and the FER library for emotion detection.
Depending on the detected emotion, different games are played to provide an interactive experience.
The code demonstrates both image processing and game logic in Python, making it a fun and educational project.
