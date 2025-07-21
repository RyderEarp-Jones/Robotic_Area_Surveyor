# Underfloor Survey Robot

This project is a small Arduino-powered robot designed to explore and map confined underfloor spaces, such as the area underneath houses. It helps reduce the need for human entry into tight or hazardous areas during construction inspections.

## Features

- **Directional Movement:** Controlled using the Serial Monitor with commands:
  - `wXX` – move forward XX cm  
  - `sXX` – move backward XX cm  
  - `aXX` – turn left XX degrees  
  - `dXX` – turn right XX degrees  

- **Obstacle Detection:** Uses an ultrasonic sensor to detect objects in front of the robot. Automatically stops when an object is closer than 10 cm.

- **LED Feedback:**
  - Green = moving forward  
  - Red = moving backward  
  - Yellow = turning  
  - Yellow + Red = obstacle detected  

- **Position Tracking:** Robot tracks and logs its position and heading as it moves.

- **Movement Logging:** Send the command `m` to view a full log of movements and positions in the Serial Monitor.

## How to Use

1. Upload the code to an Arduino-compatible board.
2. Open the Serial Monitor (9600 baud).
3. Enter movement commands (e.g., `w30`, `a90`, `d90`, `s20`).
4. Use `m` to print the robot's movement log.

---

This robot is designed for easy assembly and educational use in surveying tight construction spaces.

