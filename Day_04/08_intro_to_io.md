<!SLIDE incremental bullets>
# Input/Output

<!SLIDE center>
# What does your robot do?
## Collects information about its surroundings, discards it, and runs into walls

<!SLIDE incremental bullets>
# Input
* Any signals that come into the robot
* Digital
* Analog

<!SLIDE incremental bullets>
# Why
* So we know what our surroundings are
* So we can react to changes
* Awareness

<!SLIDE incremental bullets>
# [Analog](http://localhost:8080/class_analog_channel.html)
* Signals with a range of values
* Represented with a varying voltage

<!SLIDE incremental small bullets>
# Examples
* Rotation of a joint
* Temperature
* Light intensity
* Rate of rotation

<!SLIDE incremental bullets>
# [Digital](http://localhost:8080/class_digital_input.html) 
* Signals that are either on or off
* Varying thresholds for on/off

<!SLIDE incremental bullets>
# Examples
* Limit switch
* Encoder
* Banner Sensor

<!SLIDE incremental bullets>
# About Signals
* All signals in your robot are stored digitally
* Analog -> Digital conversion

<!SLIDE incremental bullets>
# Wait, __ALL__ Digital?
* Yes, they are encoded
* Everything in a computer is
* It's a series of 1's and 0's

<!SLIDE incremental bullets>
# Binary
* All integer numbers can be represented
* Long sequences of 1's and 0's
* Floating point is harder but doable

<!SLIDE incremental bullets>
# Benefits of Analog Signals
* Cheaper sensors
* Control the filtering

<!SLIDE incremental bullets>
# Drawbacks
* EMI
* AD accuracy
* Sampling Rate

<!SLIDE incremental bullets>
# Digital
* Clean
* Can be harder to interpret
* Harder to debug

<!SLIDE incremental bullets>
# Interrupts
## I'mma let you finish but polling is one of the most inefficient ways to watch an input OF ALL TIME! 
### - Kanye West?

<!SLIDE small incremental bullets>
# Interrupts
* Allow interrupting code when triggered
* Can trigger on
* Rising
* Falling
* Change

<!SLIDE small incremental bullets>
# ISR
* Small chunk of code that runs when interrupt triggered
* Should be FAST
* Really Fast

<!SLIDE incremental bullets>
# Output
* Motors
* Lights
* Pneumatics

<!SLIDE incremental bullets>
# But How?
* Pin is either on or off
* Electrical stuff happens
* Thing turns on or off

<!SLIDE incremental bullets>
# So Digital Output Only?
## Wait, didn't we have control of motor speed? 

<!SLIDE incremental bullets>
# Enter PWM
* Pulse Width Modulation
* Pin turns on and off 
* Used to control "inertial electrical devices"

<!SLIDE incremental bullets>
# I'm Confused
* A) Join the club, we meet on Tuesdays
* B) It's how we signal motors
* C) Smile and wave boys

.notes Yes, I'm waving my hands on how this all works. For FRC applications you need to know it exists and that's about it.

<!SLIDE incremental bullets>
# Controlling Actuators
* Define level of control
* On/Off
* Speed control

<!SLIDE incremental bullets>
# On/Off
* Use a Relay
* [Class Reference](http://localhost:8080/class_relay.html)

<!SLIDE incremental bullets>
# Speed Controller
* Use a speed controller
* Victor
* Jaguar (CAN or PWM)
* Talon 

<!SLIDE incremental bullets>
# SpeedController Class
* All speed controllers based on this
* [Class Reference](http://localhost:8080/class_speed_controller.html)


<!SLIDE incremental bullets>
# Challenge 1
* Make robot seek dark

<!SLIDE incremental bullets>


