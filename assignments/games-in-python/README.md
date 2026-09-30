# 📘 Assignment: Hangman Game

## 🎯 Objective

Build a text-based Hangman game to practice Python strings, loops, conditionals, lists, and user input. The game will select a hidden word and let the player guess letters before they run out of attempts.

## 📝 Tasks

### 🛠️ Set Up the Hidden Word

#### Description
Create the word-selection and display parts of the game. Choose a word from a predefined list and show the player which letters they have guessed correctly.

#### Requirements
Completed program should:

- Store several words in a predefined list and randomly select one for each game
- Display the hidden word as underscores, with spaces between letters (for example, `_ _ _ _` for a four-letter word)
- Replace underscores with correctly guessed letters as the game progresses


### 🛠️ Run the Guessing Game

#### Description
Let the player guess letters until they reveal the word or run out of incorrect guesses. Keep the player informed about their progress and the remaining attempts.

#### Requirements
Completed program should:

- Prompt the player to enter a letter on each turn
- Reveal every occurrence of a correctly guessed letter in the hidden word
- Track incorrect guesses and display how many attempts remain
- End the game when the player guesses the whole word or has no attempts remaining
- Display a win message when the word is guessed and a lose message when attempts run out
