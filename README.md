# JavaFX-Card-Game
## Overview:
This project is a JavaFX GUI applciation developed for a card/deck management system.

The purpose of this project was to build a visual interface that allows users to interact with an existing object-oriented model. The model classes and their relationships were already provided. The main task was to design and implement the GUI, controllers, event handling, and screen navigation.

## Gameplay Overview

This project is a JavaFX card game application where users interact with player, dealer, card, and deck objects through a graphical interface.

The application allows the user to start a game, deal cards from primary and secondary decks, select cards, view card images, track player health, play rounds, and end the game through the dealer interface.

The project focuses on applying object-oriented programming and MVC principles by separating the game data, user interface, and controller logic across model classes, FXML views, and Java controller classes.

## Related Project
This project builds on an earlier terminal-based Blackjack card game project, where the core model logic and object relationships were first introduced. This JavaFX version extends that work by replacing terminal input/output with a graphical user interface.

## How the Application Works

1. The user starts the application and enters the required player details, including the player name. The first two players are hard-coded as part of the project requirements.
   
3. The user selects **Start Game** from the login interface to begin the game.
  
5. The dealer can click the **Deal** button to deal cards to each player. Cards are dealt from the primary deck, and one player receives an additional card from the secondary deck.

6. The user can play a round to apply card damage and view each player’s remaining health in the dealer interface throughout the game.

7. The user can choose to deal cards again. When this happens, the player receiving the secondary deck card changes to the next player.

8. The user can play a round to apply card damage and view the remaining health of each player.

9. The dealer can continue dealing cards and playing rounds until only one player remains.

10. The dealer can also choose to end the game early using the **Call** button.

## Error Handling
The application includes error messages to guide the user when an invalid action is attempted.

- If the user tries to add more than four cards to a player’s hand using the **Select** button, a **"Hand is full"** error message is displayed.

- If the user tries to play a round before the players have selected a card, a **"Select a card"** error message is displayed.

- If either the primary deck or secondary deck card list runs out of cards, an **"Out of cards"** error message is displayed.

## Features
- JavaFX graphical user interface
- Login/player setup screen
- Dealer and player game views
- Primary and secondary deck management
- Card selection from deck lists and player hands
- Card image display when a card is selected
- Player health tracking throughout each round
- Round-based card damage system
- Error handling for invalid actions
- MVC-based project structure
- FXML views and Java controller classes
- CSS styling for the interface

## Project Structure
```text
.
├── src/
│   ├── controller/
│   │   ├── CardController.java
│   │   ├── DealerController.java
│   │   ├── DeckController.java
│   │   ├── LoginController.java
│   │   ├── PlayerController.java
│   │   └── PlayerWinController.java
│   │
│   ├── model/
│   │   ├── Card.java
│   │   ├── CardLibrary.java
│   │   ├── Dealer.java
│   │   ├── Deck.java
│   │   └── Player.java
│   │
│   ├── view/
│   │   ├── CardView.fxml
│   │   ├── DeckView.fxml
│   │   ├── LoginView.fxml
│   │   ├── PlayerView.fxml
│   │   ├── PlayerWinView.fxml
│   │   └── style.css
│   │
│   └── App.java
│
├── .gitignore
└── README.md
```

## How to Run the Game

### Requirements

Before running the project, make sure you have:

- Java installed
- JavaFX installed and configured
- An IDE such as Visual Studio Code or one of your preference.

### Running the Project

1. Clone this repository:

```bash
git clone https://github.com/YSeeratA86/Java-Blackjack-Card-Game.git
```

## What I Learned
This project helped me build a stronger understanding of how different responsibilities worked in an MVC-style structure, where model classes manage the game data and logic, the controller handles user interactions, and FXML files define the user interface.

- Building graphical user interfaces using JavaFX
- Connecting FXML views to Java controller classes
- Handling user actions through event-driven programming
- Managing game state across multiple screens
- Designing model classes for cards, decks, players, and dealers
- Using CSS to style a JavaFX interface
- Structuring a Java project so that the code is easier to understand and maintin.

Overall, this project helped me understand how a simple card game can be expanded into a more organised GUI application using Java, JavaFX, and MVC principles.


