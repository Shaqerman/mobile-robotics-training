<!SLIDE >
# What is Programming? #

<!SLIDE bullets incremental>
# Programming #
* The action or process of writing computer programs.
* Predetermined behavior.

.notes These are really bad definitions, I snagged them from Google's dictionary while trying to find a good way of explaining what programming was. Let's try again shall we? 

<!SLIDE bullets incremental transition=toss>
# Programming
* Programming is writing a program?
* Programming is writing code?

.notes Well, that's less than useless, maybe let's try another? Nope! still useless. Guess we're not asking the right question. 

<!SLIDE bullets incremental transition=toss>
# Why Program Stuff?
* To make it do something cool/useful
* Automate tasks



<!SLIDE bullets>
# That's Better! 
* Programming - telling a computer how to do something 

<!SLIDE bullets>
# How Do We Do It
* It's like writing a recipe

<!SLIDE bullets incremental>
# Steps
* Declare Your Ingredients
* Follow Directions
* Clean Up



<!SLIDE bullets incremental>
# Grilled Cheese - Ingredients
* 2 Slices of Bread
* Butter
* Cheese
* Tomato

.notes Normally I don't like tomato on my grilled cheese but for this example I needed to make an exception. 


<!SLIDE small>
# Grilled Cheese - Directions

1. Slice cheese into thin slices
2. Slice tomato 
3. Apply butter to bread
4. Place cheese and tomato on bread
5. Place all of that in your pan
6. Heat until cheese is melted

.notes Ok, so we have our recipe. Cool, what happens next? 

<!SLIDE center>
# Ooops
![Oops](burnt-grilled-cheese.jpg)

<!SLIDE bullets incremental>
# What happened
* Instructions were ambiguous
* Instructions were incomplete

.notes How much tomato or cheese, how much butter. How do I place it in the pan? With a person you can count on some common sense but with a computer it follows what you say exactly. Notice how I never said to remove from the pan? Or place the pan on the stove? I also never told it what a pan or a stove was. I didn't say how to heat it. I'm going to skip the cleanup step because I've made my point. 

<!SLIDE small bullets incremental>
# Takeaways

* Computers are kinda dumb
* Programs must be explicit
* Andrew eats a lot of Ramen noodles

.notes Assume that a computer is dense, really really dense. So, how can we be explicit and explain to them completely what to do in a concise manner? Also, I really don't eat Ramen noodles, they're really bad for you... too much sodium.

<!SLIDE incremental bullets>
# Programming Languages
* Typically human readable languages that can 'easily' be converted to machine readable instructions

<!SLIDE smaller> 
# What do they look like?
	@@@cpp
	int factorial(int x) {
		  if (x == 1) 
		  	return x; 
		  else 
		  	return x * factorial(x - 1);
		}
.notes Well, that looks ugly and confusing doesn't it? Well, what is it actually saying. 

<!SLIDE smaller incremental>
# Translation
* There's a function called _factorial_
* It maps its input (an integer that we just named _x_) to another integer
* Everything inside the braces is just how it maps it

<!SLIDE smaller incremental>
# A brief aside about mathematics
* This is all math
* A function is just something that takes inputs and produces an output
* We can denote this as f(x) => y
* __IMPORTANT__ if f(1) => 4 it should always map to 4. 

<!SLIDE smaller incremental>
# Math and Programming
* Almost anything that applies in math applies here too
* f(g(x)) is completely valid
* a = f(x) assigns whatever f(x) is to _a_
* b = f(x)*g(y) 
* You get the point... 

<!SLIDE bullets incremental>
# Core Concepts
* Variables
* Conditionals
* Loops

<!SLIDE bullets incremental>
# Variables
* Store _something_
* 


