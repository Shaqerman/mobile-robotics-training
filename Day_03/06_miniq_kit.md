<!SLIDE>
# Let's Get Coding

<!SLIDE bullets incremental smaller center>
# What Is This?
* Atmega 128
* Arduino Compatible
* 5x Line sensors
* Ambient Light sensor
* IR Communications
* Encoders

<!SLIDE bullets incremental smaller center>
# What's Implemented
* Motors
* LEDS
* Ambient Light sensor

<!SLIDE bullets incremental center>
# Motors
* Differential Steer
* Similar to the kitbot
* ~1 FPS

<!SLIDE bullets incremental center>
#Code 
	@@@c++
		void setLeftMotor(int speed);
	    void setRightMotor(int speed);

<!SLIDE bullets incremental center>
# LEDS
* Red
* Green
* Library supports on/off
* Hardware supports analog
* Those annoying blue ones are always on

<!SLIDE bullets incremental center>
# Code
	@@@c++
	    void setRedLED(int on);
	    void setGreenLED(int on);

<!SLIDE bullets incremental center>
# Code
	@@@c++
		analogWrite(RED_LED,value);
		analogWrite(GREEN_LED,value);


<!SLIDE bullets incremental center>
# Getting Started
* _git clone git@github.com:schreiaj/MiniQ.git_
* Copy the MiniQ folder to your Arduino Libraries folder
* Open Arduino IDE

<!SLIDE small incremental>
# Arduino
	@@@cpp
		// Include Library
		#include <MiniQ.h>

		MiniQ robot;
		void setup()
		{
			//Init serial comms
			Serial.begin(9600);
		}

		void loop()
		{
			// Your code here
		}




<!SLIDE bullets incremental center>
# Challenge
* Drive Forward for 2 seconds


<!SLIDE small incremental>
# Arduino
	@@@cpp
		// Include Library
		#include <MiniQ.h>

		MiniQ robot;
		void setup()
		{
			//Init serial comms
			Serial.begin(9600);
		}

		void loop()
		{
			robot.setLeftMotor(60);
			robot.setRightMotor(60);
			delay(2000);
			robot.setLeftMotor(0);
			robot.setRightMotor(0);
			while(1);
		}



<!SLIDE bullets incremental center>
# Challenge 2
* Drive Backward for 2 seconds

<!SLIDE small incremental>
# Arduino
	@@@cpp
		// Include Library
		#include <MiniQ.h>

		MiniQ robot;
		void setup()
		{
			//Init serial comms
			Serial.begin(9600);
		}

		void loop()
		{
			robot.setLeftMotor(-60);
			robot.setRightMotor(-60);
			delay(2000);
			robot.setLeftMotor(0);
			robot.setRightMotor(0);
			while(1);
		}


<!SLIDE bullets incremental center>
# Challenge 3
* Turn Left for 1 second

<!SLIDE bullets incremental center>
# Challenge 4
* Turn Right for 1 second

<!SLIDE bullets incremental center>
# Challenge 5
* Read Ambient light sensor

<!SLIDE small incremental>
# Arduino
	@@@cpp
		// Include Library
		#include <MiniQ.h>

		MiniQ robot;
		void setup()
		{
			//Init serial comms
			Serial.begin(9600);
		}

		void loop()
		{
			Serial.println(robot.getAmbientLight());
		}



<!SLIDE bullets incremental center>
# Challenge 6
* You used git right? 
* Roll back to Challenge 2





