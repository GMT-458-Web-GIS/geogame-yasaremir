# Ankara District Guessing Game

The **Ankara District Guessing Game** is an interactive web-based game designed to challenge and enhance players' knowledge of Ankara's districts. It offers a dynamic, map-based gameplay experience where players guess district locations, earn points based on accuracy, and receive helpful hints to refine their guesses.

---

## Features

- **Dynamic Map Integration**: Powered by the OpenLayers library, players interact with a detailed map centered on Ankara.
- **Scoring System**: Points awarded based on proximity to the target district, ranging from 50 to 1000 points.
- **Hints & Feedback**: Real-time hints and distance feedback after each guess to guide players.
- **Timer**: Each round is time-limited to 10 seconds, adding urgency and excitement.
- **Responsive Design**: Fully accessible on both desktop and mobile devices.

---

## Languages Used

### 1. HTML

Provides the structural backbone of the game.

- **Key sections**:
  - **Game Rules**: Displays instructions and rules.
  - **Map and Information Panels**: Dynamically updated with map and player statistics.
  - **Buttons**: For starting and restarting the game.

### 2. CSS

Enhances visual appeal and usability.

- **Key features**:
  - **Typography**: Uses the "Poppins" font for a clean and professional look.
  - **Responsive Design**: Adapts to different screen sizes.
  - **Interactive Effects**: Buttons and elements provide hover effects for user feedback.

### 3. JavaScript

Implements the game logic and interactivity.

- **Features include**:
  - **Map Functionality**: Integrates OpenLayers for rendering the map.
  - **Game Logic**:
    - Track guesses and calculate scores.
    - Manage round progression and scoring system.
  - **Dynamic Updates**: Real-time updates for scores, hints, and round status.
  - **Distance Calculation**: Uses the Haversine formula for precise measurements.

---

## Gameplay

### Objective

The goal is to guess the correct district on the map as accurately as possible. Players earn points based on the distance between their guess and the actual location.

### Rules

- Each round is 10 seconds long.
- The game consists of 5 rounds.
- Players make a guess by pressing the **'X' key** while hovering over the map.

### Scoring System

- **<1 km**: 1000 points
- **1-10 km**: 500 points
- **10-50 km**: 250 points
- **50-100 km**: 100 points
- **>100 km**: 50 points

### Hints

- Directional hints are provided after each guess to guide players.
  - Example: "Move further north" or "Closer to the east."

---

## Map Features

- **Markers**:
  - **Blue Marker**: Indicates the player’s guess.
  - **Red Marker**: Displays the correct district location after a guess.
- **Interactive Controls**: Players navigate the map in real-time to make guesses.

---

## How to Play

1. **Start the Game**: Read the rules and click the "Start" button.
2. **Guess Locations**:
   - Use the map to identify the district.
   - Press the **'X' key** to lock in your guess.
3. **Hints and Feedback**:
   - After each guess, see your score, distance from the target, and helpful hints.
4. **Final Score**: At the end of 5 rounds, your total score is displayed.
5. **Replay**: Click "Restart" to play again and improve your score!

---

## Technical Details

### Dynamic Map Integration

- The OpenLayers library powers the map.
- Features include base layers from OpenStreetMap, vector layers for guesses and targets, and real-time interaction.

### Distance Calculation

- The **Haversine formula** ensures accurate measurement of the distance between the player’s guess and the target district.

### Responsive Design

- The game adapts to different screen sizes, ensuring smooth play on both desktop and mobile devices.

### Real-Time Feedback

- Immediate updates for:
  - **Scores**
  - **Distance to the target**
  - **Incremental hints for better accuracy**

---
###My webpage:https://gmt-458-web-gis.github.io/geogame-yasaremir/
