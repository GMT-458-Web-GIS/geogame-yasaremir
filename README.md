
1. Web Page Layout
The game's web page is structured as follows:

Header Section:

Displays the game's title: "Ankara İlçe Tahmin Oyunu".
Provides a brief description of the game's rules.
Game Area:

Includes an interactive OpenLayers map displayed within the <div id="map">.
Users interact with the map to make guesses by pressing the "X" key.
The background map is sourced using OpenLayers and styled with interactive markers.
Sidebar/Information Section:

Displays the game status, including:
Score (<p id="score">): Tracks the player's points.
Round Number (<p id="round">): Indicates the current game round out of 5.
Messages (<p id="message">): Provides instructions or feedback.
Hint (<p id="hint">): Offers directional guidance based on the user's guesses.
Distance (<p id="distance">): Shows the distance between the guess and the target.
Includes a restart button (<button id="restartButton">).
2. Game Description and Geo-Component
Description: This is a geographic knowledge and accuracy game focused on Ankara's districts. The user guesses district locations on a map to score points.

Game Execution:
Players are given a random district target location for each round.
Players navigate the map and press the "X" key to lock in their guess.
Points are awarded based on the proximity of the guess to the actual district location.
Hints are provided to assist in narrowing down the target location.
The game concludes after 5 rounds.
Winning Points System:

Proximity Scoring:

< 1 km: 1000 points
1–10 km: 500 points
10–50 km: 250 points
50–100 km: 100 points
100 km: 50 points

Timer-Based Gameplay:

Each round has a 10-second time limit.
Players must guess before the timer runs out; otherwise, they lose the round.
Geo-Component:

Utilizes OpenLayers to render a map of Ankara.
Allows dynamic interactivity:
Detecting mouse pointer position (pointermove event).
Mapping guesses and calculating distances between guessed and target locations.
3. Chosen JavaScript Library
Library: OpenLayers

Functionality Used:
Interactive Map:
Rendering map tiles using ol.layer.Tile and OpenStreetMap as the base map.
Geographic Calculations:
Distance calculation between the guessed and target locations using spherical trigonometry.
Dynamic Features:
Adding guessed and target markers (ol.Feature).
Styling features dynamically based on proximity.
Event Handling:
Pointer movement (pointermove) to track the current position of the mouse.
Keypress events (keydown) for capturing the user's guess action.
Projection Support:
Using ol.proj to convert between geographic (latitude/longitude) and projection coordinates.
Implementation Highlights:

The library is key for managing geographic elements and interactions.
The game logic heavily relies on OpenLayers' built-in methods for rendering and manipulating geospatial data.
