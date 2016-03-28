# The Flying Platypi (FRC2655) - 2016 Robot Code - Sir Lance-A-Bot

![Sir Lance-A-Bot](http://i.imgur.com/7AbfNr6.jpg "Sir Lance-A-Bot")

This repository contains all of the robot code for our 2016 competition robot. Some of the code's features are listed below.

  - All robot code is written in LabVIEW
  - Our code integrates a script interpreter built into the driver station
    - The script manager interprets CSV files on the driver station PC and sends them to the robot at the beginning of a match
    - Each valid command is interpreted in the autonomous LabVIEW code and executed in the order specified in the CSV file
  - The control scheme is built for tank drive controlled with a PlayStation 2 controller
  - Talon SRXs are used in a Master-Slave speed feedback configuration to provide the driver with precise control
  - A "Drive Straight" function was implemented to aid in crossing defenses during teleop
  - Both the IMU and Gyro/Accel board are supported in the code and can be swapped by a single boolean in Robot Main.vi

Feel free to clone/fork the project and take a look around! Every effort has been made to keep the code as modular as possible. If you have any questions, open a request! IMU code was integrated from [this](https://github.com/juchong/ADIS16448-RoboRIO-Driver) repository.
