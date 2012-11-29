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
* Must be declared before they can be used

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
# Example
	@@@cpp
		int randomNumber(int seed) {
			  return 4;
			}

<!SLIDE bullets small incremental>
# Loops
* Two main options
* _for_
* _while_

<!SLIDE bullets small incremental>
# _for_
* Syntax for([initialize];[increment];[endCondition]){[content]}

<!SLIDE bullets small incremental>
# _for_ ... explained
* _initialize_ is run when your loop starts
* _increment_ runs each iteration
* _endCondition_ is checked each iteration, if it is false loop exits
* _content_ is what is run each iteration

<!SLIDE bullets small incremental>
# Example
	@@@cpp
		int i;
		for(i=0;i<10;i = i+1)
		{
			printf("%d ", i);
		}

<!SLIDE bullets small incremental>
# Output
* 0 1 2 3 4 5 6 7 8 9
* Why no 10? 
* Why 0?

<!SLIDE bullets small incremental>
# _while_
* Syntax while(condition){[content]}
* Do something until condition is false

<!SLIDE bullets small incremental>
# Example
	@@@cpp
		while(1==1)
		{
			printf("To infinity...\n"):
		}
<!SLIDE bullets small incremental>
# Output 
* To infinity...
* To infinity...
* To infinity...
* To infinity...
* To infinity...
* To infinity...
* To infinity...
* To infinity...
* To infinity...
* To infinity...

<!SLIDE bullets small incremental>
# Infinite Loops
* Actually, useful.
* Can be broken out of other ways (_break_)
* Doing something forever (Operating Systems?)

<!SLIDE bullets small incremental>
# Conditions
* Syntax Options:
* if([condition]) {[code]}
* if([condition]) {[code]} else {[otherCode]}

<!SLIDE bullets small incremental>
# Example
	@@@cpp
		if(randomNumber(123456) == 4)
		{
			printf("You won!\n");
		}
		else
		{
			printf("Nope!\n")
		}

<!SLIDE bullets small incremental>
# Output
* You won!
* _randomNumber_ always returns 4... It's a bad random number generator

<!SLIDE bullets small incremental>
# Comments
* // is a single line comment
* /* starts a multiline comment
* */ ends a multiline comment

<!SLIDE bullets small incremental>
# Example
	@@@cpp
		// This is a single line comment
		/* This
			Is
			A 
			Multiline Comment
			...
			Also, Sparta
		*/
		/*This is legal too */
		randomNumber(/*Who cares what we put here*/ 2); 

<!SLIDE bullets small incremental>
# On Whitespace
* Whitespace doesn't matter all that much
* Delimits keywords

<!SLIDE bullets small incremental>
	@@@cpp
		int a = 5;
		int a=5;
		int 
			b
				=
					6;

<!SLIDE bullets small incremental>
# Uses for whitespace
* Lining things up
* Readability

<!SLIDE bullets small incremental>
# Keywords
* [http://en.wikipedia.org/wiki/C_(programming_language)#Keywords](http://en.wikipedia.org/wiki/C_(programming_language)#Keywords)

<!SLIDE bullets small incremental>
# Pointers
* I'm going to wave my hands on this
* Until we need them I prefer not to mention them
* Won't be important if you use Java