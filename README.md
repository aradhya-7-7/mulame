
# Mulame - A Multiplayer Coin-Collecting Game

Mulame is a simple, real-time multiplayer game built using vanilla JavaScript and Firebase. Players can navigate around the game map, collect coins, and customize their character’s name and color. Firebase is used for authentication and real-time database synchronization, allowing players to see each other’s movements in real time.

## Features

- **Real-time multiplayer:** See other players moving around the game map.
- **Firebase Authentication:** Players are automatically signed in anonymously to Firebase.
- **Coin Collection:** Players can collect coins that randomly spawn on the map.
- **Customizable characters:** Players can change their in-game name and character color.
- **Real-time updates:** All movements and coin pickups are synchronized in real time across all players.

## Demo

![Game Screenshot](![screenshot](images/screenshot.png))

## Project Structure

- `index.html`: Main HTML structure for the game.
- `styles.css`: Styles and layout of the game and UI elements.
- `app.js`: Main game logic including player movement, coin collection, and Firebase interactions.
- `KeyPressListener.js`: A utility class for handling keyboard input.
- `images/`: Folder containing all game assets like the map, characters, coins, and shadows.

## Firebase Setup

This project uses Firebase for real-time updates and anonymous authentication. To set up Firebase:

1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
2. Enable Firebase Authentication with Anonymous sign-in.
3. Set up a Realtime Database with read/write rules for players and coins data.
4. Replace the Firebase config object in `index.html` with your project credentials.

js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};


## Getting Started

To run this game locally, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/mulame.git
   ```
2. Navigate to the project directory:
   ```bash
   cd mulame
   ```
3. Add your Firebase config to the `index.html` file.
4. Open `index.html` in a web browser.

No server setup is required since Firebase handles the backend.

## Game Instructions

1. Upon loading the game, you’ll be automatically signed in anonymously via Firebase.
2. Use the arrow keys to move your character around the map.
3. Collect coins that randomly appear on the map by moving over them.
4. You can change your player’s name and color using the input fields and buttons in the UI.

## Technologies Used

- **HTML5**
- **CSS3**
- **Vanilla JavaScript**
- **Firebase (Authentication, Realtime Database)**

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```
