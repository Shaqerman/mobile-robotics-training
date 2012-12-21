<!SLIDE incremental bullets>
# Feedback Systems

<!SLIDE incremental bullets>
# What
* When you use input to drive your output

<!SLIDE incremental bullets>
# Why
* Allows inputs to drive outputs
* Enable better control of system

<!SLIDE incremental bullets>
# How
* out = f(input)
* You need sensors

<!SLIDE incremental bullets>
# Let Me Reiterate
## YOU NEED SENSORS

<!SLIDE incremental bullets>
# So Far
	@@@cpp
		void loop()
		{
			robot.setLeftMotor(60);
			robot.setRightMotor(60);
			delay(1000);
			robot.setLeftMotor(0);
			robot.setRightMotor(0);
			while(1);
		}

<!SLIDE incremental bullets>
# How far does this go?
* 2'?
* 4'?
* 1'?

<!SLIDE incremental bullets>
# Well?
* It depends
* ^ This is a terrible answer

<!SLIDE incremental bullets>
# Driving To Specific Light Value
* Assume there is a light gradient
* As we drive forward it get's darker
* Drive to 50% dark

<!SLIDE incremental bullets>
# Simple Approach
	@@@cpp 
		void loop()
		{
			robot.setLeftMotor(60);
			robot.setRightMotor(60);
			if(robot.getAmbientLight() < threshold)
			{
				robot.setLeftMotor(0);
				robot.setRightMotor(0);
			}

		}

<!SLIDE incremental bullets>
# Problems?
* What if we drive past it?
* We stop too late
* This is called overshooting

<!SLIDE incremental bullets>
# So what can we do?
* lightIntensity is a function of distance...
* distance is a function of motor velocity and time...
* Can we combine these?

<!SLIDE incremental bullets>
# YES! 
* Let's feed ambient light into our velocity
* Sure, why not

<!SLIDE smaller incremental bullets>
# Hijinks and Shenanigans
	@@@cpp
		void loop()
		{
			int speed = 
				(robot.getAmbientLight() - threshold)*scale;
			robot.setLeftMotor(speed);
			robot.setRightMotor(speed);
		}

<!SLIDE smaller incremental bullets>
# What?
* threshold stays the same
* scale is just a transformation
* At threshold speed -> 0
* Past it? 
* Motors reverse 


<!SLIDE incremental bullets>
# Sweet! 
* So, what's the problem?
* As light approaches threshold ...
* speed approaches 0 ... 
* unless scale is big.

<!SLIDE incremental bullets>
# So, make scale huge
* Just keep swimming...
* aaaand overshoot!

<!SLIDE incremental bullets>
# What else can we do? 
* What if we accumulated error over time.

