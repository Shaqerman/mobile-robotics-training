<!SLIDE incremental bullets>
# Filtering

<!SLIDE incremental bullets>
# Why Filter
* Signals are noisy
* Isolate frequencies
* Anti-Aliasing (smoothing)

<!SLIDE incremental bullets>
# Noise
* $^&% in ,$^&% out
* Clean up your signal

<!SLIDE incremental bullets>
# Isolation
* Strip erroneous data out
* Allow you to operate on just what you need

<!SLIDE incremental bullets>
# Smoothing
* Less noise in systems using data

<!SLIDE incremental bullets>
# How Do?
* Ask your local EE
* No, seriously. 

<!SLIDE incremental bullets>
# We Don't Have One
* WPILib has some filtering 
* [Keyword - SOME](http://localhost:8080/class_analog_channel.html)
* Simple cleaning of signal

<!SLIDE incremental bullets>
# Simple Stuff
* CK15 Shooter
* Controller/Motor combo led to oscillations

<!SLIDE smaller incremental bullets>
# Quick and Dirty
	@@@cpp
		output = prevOutput*(1-weight) + calcOutput*(weight);