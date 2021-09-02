// Emerson Racca
// 09/01/21
// Lab 3d: Compound Interest


/*
Create a program that makes use of a regular function that calculates and returns the amount in an account earning monthly compound interest after a given amount of time.  Use the formula found here:

A = P(1 + r/12)^(12t) (Links to an external site.)

1. Tell the user what the program does.
2. Prompt the user for the Principal (double), annual rate as a percent (example: 3.5 for 3.5%) , and time in years (int).
3. Display the Amount rounded off to two places.

Please separate the function interface from the implementation and test thoroughly.

--------

Choosing the compounding frequency option, this App's data was verified with -- https://www.wolframalpha.com/calculators/interest-calculator
*/

#include <iostream>
#include <iomanip>
#include <cmath>


using namespace std;

double computeFutureValue (double P, double r, int t);

int main()
{
    double principal, annualRate;
    int timeInYears;
    
    
    cout << "Compound Interest Calculator\n\n";
    cout << "This app calculates and returns the amount in an account\n";
    cout << "earning monthly compound interest after a given amount of time.\n\n";
    
    cout << "What is the Principal amount? ";
    cin >> principal;
    
    cout << "\nWhat is the Annual Rate (example: 3.5 for 3.5%)? ";
    cin >> annualRate;
    
    annualRate = annualRate / 100;
    
    cout << "\nWhat is the Time in year(s)? ";
    cin >> timeInYears;
    
    cout << fixed << setprecision(2);
    cout << "\n\nYour new Principal after " << timeInYears << " year(s) is $" << computeFutureValue(principal, annualRate, timeInYears) << " ." << endl;
    
  
}

double computeFutureValue (double P, double r, int t){
    return (P * (pow ((1 + (r / 12.0)), (12.0 * t)))); 
}
