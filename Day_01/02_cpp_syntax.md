<!SLIDE bullets incremental>
# C++? #
* Variables
* Functions
* Loops
* Conditionals

<!SLIDE small bullets incremental>
# Variables
* Start with a letter or underscore
* Can contain any number of numbers, letters, or underscores after that
* May not contain spaces, periods, commas, or other punctuation
* Must have a type declared

<!SLIDE small bullets incremental>
# Types?
* Tell what type of data is in the variable
* Several default types
* Can create your own

<!SLIDE smaller bullets incremental>
# Built in Types
* __char__ stores a small number, smallest addressable unit of memory on the machine
* __int__ stores integer numbers, usually 16 bits in size 
* __long__ stores larger numbers, 32 bits typically
* __float__ stores single precision floating point numbers
* __double__ stores double precision floating point numbers
* Sizes vary... __long__ __long__ > __long__ > __int__  and __double__ > __float__

<!SLIDE small incremental>
# Declaring variables
	@@@cpp
		int numberOfCats; // Without an initial value
		int numberOfDogs = 2; // With an initial value

<!SLIDE bullets small incremental>
# Important Things
* All statements end in a ;
* Syntax is [type] [name];
* Alternately [type] [name] = [value];

<!SLIDE bullets small incremental>
# Functions
* Syntax is [returnType] [name] \([arg1Type] [arg1Name]...[argNType] [argNName]\)
	{
		[content]
	}
* Valid names are same as variable names
* May not return anything, in that case use _void_

<!SLIDE bullets small incremental>
	@@@cpp
		int factorial(int x) {
			  if (x == 1) 
			  	return x; 
			  else 
			  	return x * factorial(x - 1);
			}
