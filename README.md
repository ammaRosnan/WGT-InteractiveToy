# WGT-InteractiveToy
A group project where we designed a 2-Player toy to entertain children on long car journeys, without relying on a screen. Each player held a steering wheel and had to react to the movements of the vehicle their were in, racing to mimic its motion before their opponent. The full system consisted of:
- 2 Xiao ESP32-S3s
- 1 Inertial Measurement Unit
- 2 Rotary Encoders
- 2 LCD Displays
- 4 Buttons

One of the two Xiao ESP32-S3s acted as the "Master Board," fitted with the IMU to detect directional changes in the device's movement. These were processed to classify the motion of the vehicle as accelerating, decelerating, turning left, or turning right. The two rotary encoders (mounted on each player's wheel) captured the players' own steering movements, and the player that replicated the vehicle's motion first scored a point. The two Xiao boards communicated wirelessly, allowing the Master Board to relay the target movement and receive each player's response in sync.

Instead of using pedals for accelerating and braking we used buttons. This kept the design compact, portable, and removed the need for loose cables that could pose a strangulation risk. Each player had their own LCD display, showing the current score along with contextual feedback, such as a green light for the player that reacted fastest to a given movement. 

<p align="center"><img height="500" alt="final" src="https://github.com/user-attachments/assets/1034722b-d729-4df2-aea5-7defd921be6b" /></p>
<p align="center"><b>Final Product</b></p>

<p align="center"><img height="450" alt="bothBoards" src="https://github.com/user-attachments/assets/fe378513-3777-4644-9cee-f1cfc94a6583" /></p>
<p align="center"><b>KiCad Diagrams for both wheel's boards</b></p>

<p align="center"><img height="300" alt="wheelModel" src="https://github.com/user-attachments/assets/7f6cce40-c597-455c-9db5-2e50bca94a80" /><img  height="300" alt="neckConnector" src="https://github.com/user-attachments/assets/4a306173-1ddd-4482-9b3a-342193587169" /></p>
<p align="center"><b>3D models of the wheel components</b></p>


