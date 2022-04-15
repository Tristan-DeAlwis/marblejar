Taken from https://compsci.sites.tjhsst.edu/CS2C/U1/using.html

Using a Class
Marble Jar Puzzle
Objective
Using simulations to solve a puzzle.
To help in solving this kind of puzzle, it will be useful to have a class which simulates the operations allowed on a jar of marbles.
class MarbleJar
{
public:
	MarbleJar(int black, int white);	// initializes jar contents
	String DrawMarble ( );	// draws and returns color
	void AddMarble (String color);	// adds marble to jar
	Boolean IsEmpty ( );	// returns true if empty
private:
	int myNumberBlack, myNumberWhite;	// marbles in the jar
	int myRandom ( );	// random number generator
};
It is important to note that this class provides the necessary operations for manipulating a jar and only those operations. The person is only allowed to remove a random marble, add a marble of a specific color, and know when the jar is empty (equivalent to picking up the jar and shaking it to see if there is anything inside.
LabA : Probability Simulation
Assignment
Suppose a jar contains the same number of black and white marbles. If you reach in and pull out two random marbles, are they more likely to be the same color or different colors?
Using the MarbleJar class,  write a program that will help you solve the problem. Your program should prompt the user for the initial number of marbles of each color. Then it should repeatedly draw two marbles, noting when they are the same color and then returning them to the jar. It should do this some constant number of times (say 1000) and then output the number and percentage of each type of result.
Sample Run
How many marbles of each color in the jar? 100

	Out of 1000 trials
		same colors drawn 479 times
		different colors drawn 521 times
	That means they were the same 47.9% of the time
Analysis
Once you have your program working, answer the following questions:
Perhaps using repeated simulations as a guide, what is the answer to this puzzle? Are the two marbles more likely to be the same color or different colors. Can you explain why?
