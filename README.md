Maze Game Frontend
This repository contains the frontend code for the hand-gesture-controlled maze game, along with integration points to the backend API.

Project Overview
The frontend is a lightweight web application responsible for rendering the maze and interpreting navigation commands received from the backend API, which predicts maze movements based on real-time hand landmark detection and machine learning.

Frontend & Backend Integration
Frontend renders the maze and captures user inputs.

Backend runs a FastAPI server that processes hand landmarks using ML models and returns predicted maze actions.

Link Between Frontend and Backend:
The file api-call.js handles all communication with the backend API. It sends landmark data to the backend /predict endpoint and receives navigation commands such as "up", "down", "left", or "right" to control the maze accordingly.

Files and Description
File Name	Description
index.html	Main HTML page for the maze game UI
maze.js	Core maze logic and rendering
keyboard.js	Keyboard event handling for local control
api-call.js	Handles API requests/responses to backend
mp.js	MediaPipe or helper JS (if used)
jquery.js	jQuery library for DOM manipulation
Box2dWeb.min.js	Box2D physics engine for maze dynamics
ball.png	Maze ball sprite
brick.png	Brick texture for maze walls
concrete.png	Concrete texture background
License.md	License information

Branch Structure
master: Contains the complete frontend code.

backend(branch) : Contains the backend code including FastAPI server, ML models, and monitoring, integrated or linked with the frontend.

How to Run Locally
Start the backend API server (FastAPI app) and ensure it is running on http://localhost:8000.

Open index.html in a modern web browser.

The frontend captures hand landmarks, sends them via api-call.js to the backend, receives maze navigation commands, and updates the maze in real-time.

Demo Video
![Maze_using_hand_signs](https://github.com/user-attachments/assets/29b236fe-47cd-4df0-acc8-39e1f5a23e14)




Author
Eng. Khalid Ahmed Mohamed
