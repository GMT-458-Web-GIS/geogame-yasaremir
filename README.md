My webpage:https://gmt-458-web-gis.github.io/geogame-yasaremir/
Purpose and Objective
The main objective of the game is to challenge players to identify districts in Ankara based on given hints. The game promotes learning about Ankara’s geography while maintaining an element of fun through competitive scoring and time-bound rounds. The player’s ability to make accurate guesses is rewarded with points, encouraging repeated attempts to improve geographic knowledge and accuracy.

Technologies Used
1. HTML
HTML is the foundation of the game’s structure. It organizes the game’s various sections and elements into an easily navigable layout, ensuring players have a clear understanding of the game interface. Key components include:

Game Rules Section: Displays the instructions and rules at the start.
Map and Information Panels: Dynamically updated sections show the interactive map and player statistics, such as score and round progress.
Action Buttons: Used for starting and restarting the game with clear visual cues.
2. CSS
CSS provides the visual styling that makes the game both attractive and functional. The styling ensures a smooth user experience through:

Typography: The "Poppins" font from Google Fonts gives the interface a modern and professional look.
Color Scheme: A light background  and contrasting text color  enhance readability.
Responsive Design: The layout adjusts automatically to different screen sizes, ensuring the game is fully accessible on both desktop and mobile devices.
Interactive Effects: Hover effects on buttons provide instant visual feedback, improving the overall user interaction.
3. JavaScript
JavaScript powers the game’s logic, interactivity, and functionality. It is responsible for:

Map Integration: The OpenLayers library enables a dynamic and interactive map interface.
Game Logic:
Players navigate the map and make guesses by pressing the 'X' key while hovering over the map.
Scores are calculated based on the proximity of the player’s guess to the correct district location.
Five rounds are played in each game session, with a new target location presented for every round.
Timer Mechanism: A 10-second countdown per round adds urgency and keeps players engaged.
Dynamic Updates: The game dynamically updates and displays scores, round progress, distance to the target, and hints as the game progresses.
Gameplay Mechanics
Objective
The goal is to guess the district’s location on the map with the highest accuracy possible, earning more points for closer guesses.

Rules
Each round lasts 10 seconds, during which the player must make a guess.
The game consists of five rounds, and at the end of the game, the total score is displayed.
Players make their guess by hovering over the map and pressing the 'X' key.
Scoring System
Points are awarded based on how close the player’s guess is to the actual district location. The scoring system is as follows:

Less than 1 km: 1000 points
1 km - 10 km: 500 points
10 km - 50 km: 250 points
50 km - 100 km: 100 points
More than 100 km: 50 points
Hints
After each round, the game provides directional hints to help the player refine their guesses in subsequent rounds. Examples of hints include suggestions like:
“Move further north.”
“Closer to the east.”
Map Features
The interactive map is the central feature of the game, powered by OpenLayers:

The map is centered on Ankara and provides a zoom level suitable for district-level exploration.
Blue Marker: Represents the player’s guess location.
Red Marker: Displays the correct district location after each guess.
Technical Implementation
1. Dynamic Map Integration
The game leverages the OpenLayers library to deliver a fully interactive and visually appealing map:

Base Layer: A tile layer sourced from OpenStreetMap serves as the foundation for the map display.
Vector Layers: Separate layers are used to display the guessed location and the actual district location, ensuring clarity for the player.
Event Listeners: Mouse movements and key presses are tracked in real-time to capture and process the player’s guesses.
2. Distance Calculation
To calculate the distance between the guessed location and the actual district, the Haversine formula is used. This ensures precise measurement of the great-circle distance, essential for accurate scoring.

3. Responsive Design
The game’s layout is designed to work seamlessly across devices. Whether played on a desktop computer or a mobile phone, the interface adjusts dynamically for optimal usability.

4. Real-Time Feedback
Players receive instant feedback after every guess. Key updates include:

Distance between the guessed and actual location.
Hints for refining future guesses.
Incremental score updates displayed on the interface.
Game Flow
Start: Players begin by reading the rules and clicking the "Start" button.
Rounds: Each round introduces a new target district. Players have 10 seconds to make a guess.
Feedback: After every round, players see their score, distance from the target, and helpful hints.
Game End: After five rounds, the final score is displayed. A “Restart” button allows players to try again.
