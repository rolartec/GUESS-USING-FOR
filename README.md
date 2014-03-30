GUESS-USING-FOR
===============
GUESSING NUMBER USING "FOR"


//By Reina Olarte

//Guessing Number  Using FOR

import java.util.Scanner;

						// imports the Scannner Class
import java.util.Random;
	
//import the random class


public class GuessingFor2
{

	public static void main(String[] args)
	
	{
		
		for(int i=0; i<3; i++)
		{
		
		// Create the Scanner to input the number
		Scanner input = new Scanner(System.in);
		// Create the Random number
		Random randomNumber = new Random();
		
		//Declaring the variables 
		int Usernumber;
		int computerNumber;
		computerNumber = 0 + (int)(Math.random() *10);
		
		System.out.println("Welcome to the Guessing game\nEnter a digit from 0 to 10:");
		Usernumber = input.nextInt();
		if (computerNumber == Usernumber)
		{
			System.out.printf("You Guessed the right number\n\n");
			System.out.printf("Your number %d, Random number %d\n\n" , Usernumber, computerNumber);
		}

		else
			{
				if (computerNumber < Usernumber)
				{
					System.out.printf("You Guessed to High\n\n");
					System.out.printf("Your number %d, Random number %d\n\n" , Usernumber, computerNumber);
				}
				else
				{	System.out.printf("You Guessed to Low\n\n");
				System.out.printf("Your number %d, Random number %d\n\n", Usernumber, computerNumber);
				}	
				
			}
		
			}  // END FOR
}	//End main

}	//End class

