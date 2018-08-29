# Lab1
//Jorge Martinez
//CPSC 121 Lab 1
//8/29/2018

#include <iostream>
using namespace std;

int main()
{
  // Identifying Variables
  int total = 0;
  int coins = 0;
  int quarters = 0;
  int dimes = 0;
  int nickels = 0;
  int pennies = 0;
  //Ask user for input
  cout << "Please enter the number of cents";
  cin >> total;
  //Setting Values to Variables
  quarters = total / 25;
  dimes = total % 25 / 10;
  nickels = total % 25 % 10 / 5;
  pennies = total % 25 % 10 % 5 / 1;
  // Display output to user
  cout << quarters << " quarters," << dimes << " dimes," << nickels << " nickels," << pennies << " pennies" << endl;
  coins = quarters + dimes + nickels + pennies;
  cout << "The total number of coins used was " << coins << endl;
  return 0;
}
