
GeoGame Design Explanation
GeoGame is a browser-based, interactive game where players attempt to locate a randomly selected target location on a map.The primary goal in GeoGame is for the player to locate a random target location on the map. Players get points based on the proximity of their guess to the target. The closer the guess, the higher the points scored. The game uses the OpenLayers library for its mapping component, allowing players to make selections by clicking on the map to guess the target location. The scoring system awards or deducts points based on how close the player’s guess is to the target.

1. Requirements and Frontend Layout
Game Requirements
To ensure GeoGame is fun and functional, a few key requirements have been outlined:

Mapping Component: The core of the game is an interactive map where users can zoom, pan, and click to locate the hidden target.
Target Location: At the start of each game or after resetting, a randomly generated geographic location is chosen, which the player attempts to find.
Scoring System: A scoring mechanism where players earn points based on their proximity to the target. Close clicks yield higher points, while distant guesses may result in fewer points or even point deductions.
Feedback System: Instant feedback is provided after each click, letting the player know if they were close to the target or if they need to keep trying.
Reset Function: A button allowing players to restart the game, randomize the target location, and reset the score.
Frontend Layout
The user interface is designed to be simple and easy to understand, allowing players to focus on the map and finding the target:

Map Area: Occupies the main part of the layout and is the interactive space where players make guesses by clicking on the map.
Score Display: Positioned above the map, it shows the player’s current score, updating with each guess.
Reset Button: Located below the map, it lets players restart the game, reset the target location, and refresh the score.
--------------------------------------
| GeoGame - Click the Target!        |
| Score: X                           |
--------------------------------------
|                                    |
|           Map Area                 |
|                                    |
--------------------------------------
|            Reset Game              |
--------------------------------------
Top of the Page: The game’s title ("GeoGame - Click the Target!") is displayed at the top, quickly orienting players.
Score Display: Directly below the title, it shows the current score as “Score: X,” where X represents the player’s current points.
Map Area: Occupies the majority of the layout and serves as the main interactive area where players make their guesses.
Reset Button: Located just below the map, providing a quick way to restart the game.

README Content
The README file should contain detailed information about the game’s usage and development process. This file can include the following sections:

Requirements List: A checklist of all game functionalities (e.g., map, scoring, feedback, and reset functions).
Chosen Library: OpenLayers is chosen as it provides the geographic interaction features needed for the game format.
Layout Drawing: A simple visual or text-based wireframe showing the position of each element (map, score display, reset button) on the page

Library Choice: OpenLayers
Why OpenLayers?
OpenLayers offers a robust set of tools for creating interactive map-based web applications. It allows for zooming, panning, clicking, and measuring distances, all of which are critical features for this game. While other libraries like Leaflet could also be used, OpenLayers provides enhanced flexibility and more built-in functions for managing geographic projections, making it ideal for the GeoGame’s requirements.

How OpenLayers is Used:
OpenLayers will initialize the map, manage geographic projections, and track clicks to calculate distances to the target location. This allows us to deliver an engaging and accurate experience as players attempt to find the hidden target.
