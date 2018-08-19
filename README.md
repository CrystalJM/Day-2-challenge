Day 2 Challenge help.
package Practice;

import java.util.Scanner;

public class practice {
	public static void main(String[] args) {
/**********************************************************************************
 * this is pretty much how i worked out the math part, i think i got the math. 
		 * mealCost is the same as 12 this is the base cost to which the percentages must be added
the tip is the same as 20, this is a percentage. 
tax is also a percentage which is 8.
first divide the percentage (20) by 100. this comes to 0.2, then multiply that by the base cost
of the meal which is 12. the answer will be 2.4

it is 12 times the answer to 20 divided by 100. the anser is 2.4

do the same for tax

divide 8 by 100. this is 0.08. then multiply it by 12. the answer is 0.96.

the the total cost is the meal cost (12) plus tip (2.4) plus tax (0.96

the answer is 15.36. 

.36 is less than .50 so it rounds to just 15. 

got help with percentages from:
https://sciencing.com/work-out-percentage-using-calculator-7598661.html
***************************************************************************************/
Scanner scan = new Scanner(System.in); { 
	
	//the following code is given.
	
int tip_percent = scan.nextInt();
int tax_percent = scan.nextInt();
double meal_cost = scan.nextDouble();

//this looks like a mess...even to me.
int tip = tip_percent / 100; 
int mealAndTip = tip * meal_cost; // apparently you cannot perform an operation on a double and an int? i have tried to look this up.
//im trying to add the tip percent to the total meal cost.
int tax = tax_percent / 100;
int mealAndTax = tax * meal_cost;//this also gives an "cannot convert double to int" error.
//same thing here just with tax.

int totalCost = mealAndTip + mealAndTax;
//adding both to the total cost of the meal. 
System.out.println(totalCost);
//help. . . 
