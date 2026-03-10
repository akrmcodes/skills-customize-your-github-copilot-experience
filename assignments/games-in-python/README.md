
# 📘 Assignment: Games in Python (Hangman Challenge)

## 🎯 Objective

Build a command-line Hangman game to practice core Python skills such as loops, conditionals, string handling, lists, and user input.

## 📝 Tasks

### 🛠️ Game Setup and State Tracking

#### Description
Set up the initial game by selecting a secret word, creating variables to track guesses, and showing the player the starting progress.

#### Requirements
Completed program should:

- Randomly select a word from the provided `words` list.
- Initialize game state variables such as `guessed_letters`, `incorrect_guesses`, and `max_incorrect`.
- Display the hidden word as underscores (for example: `_ _ _ _ _`) at the start of the game.
- Show the number of incorrect guesses remaining.

### 🛠️ Gameplay Loop and End Conditions

#### Description
Implement the main loop where the player enters guesses, the game state updates each turn, and the game ends with a clear result.

#### Requirements
Completed program should:

- Prompt the user for one letter per turn and normalize input (for example, convert to lowercase).
- Validate input to ensure it is a single alphabetic character.
- Update guessed letters and reveal correctly guessed positions in the word.
- Increase incorrect guess count for wrong guesses and show remaining attempts.
- End the game when the word is fully guessed or attempts run out.
- Display a clear win/lose message and reveal the secret word at the end.
