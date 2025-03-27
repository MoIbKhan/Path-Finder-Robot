Robot demo video: https://files.fm/f/4k7fv7643t

Autonomous Path Detection Robot  

An Arduino-based robot that navigates obstacles autonomously using ultrasonic sensors and servo motors.  

Features  
- **Obstacle Avoidance**: Uses HC-SR04 ultrasonic sensor to detect objects within 15cm.  
- **Dynamic Movement**: Servo motor scans left/right to find clear paths, with 4 DC motors for smooth navigation.  
- **Efficient Logic**: Prioritizes longer unobstructed paths (right or left) to minimize collisions.  

Hardware  
- Arduino Uno  
- HC-SR04 Ultrasonic Sensor  
- Servo Motor (for scanning)  
- L293D Motor Shield (controls 4 DC motors)  

Code Highlights  
- **Sensor Integration**: `NewPing.h` library for accurate distance measurement.  
- **Motor Control**: `AFMotor.h` library to manage motor speed/direction.  
- **Algorithm**:  
  - Stops and reverses if obstacle is too close.  
  - Scans surroundings and turns toward the clearest path.  
How to Use  
1. Upload the `.ino` file to your Arduino.  
2. Power the robot (battery/USB).  
3. The robot will move forward until an obstacle is detected, then autonomously reroute.  


