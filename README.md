# Control-robot-movement-using-a-website
In this task we have made a website with buttons to control the robot, either move forward/backward or turn right/left
The way this work, we made a new table name "movement" in the database, and the ESP32 code Movement.ino in Task4 will read the data from the database frequently using GET method.
when the user click the forward button, the website will send "forward" to the database and ESP32 will read it to move forward, and when the user click the right button, we will send "right" to the database and ESP32 will also turn right.
As you see in the image above, we also register how long did the user pressed the button, he clicked the forward button for 3.3 seconds and clicked the right button for 1.6 seconds. This is useful later if we want the robot replay what the user clickd before.
