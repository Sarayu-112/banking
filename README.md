#include<iostream>
#include<stdlib.h> // Included for using the exit() function
#include<conio.h> // Included for using getch() function for pausing the screen
#include<string>
using namespace std;

// Structure to represent a bank account
struct bankmanagement
{
    int accno; // Account number
    string name, address; // Account holder's name and address
    char actype; // Account type (saving or current)
    float amount; // Account balance
    
    // Function declarations for various operations on bank accounts
    bool checkavailabilty(); // Check if the account slot is available
    bool searchaccount(int); // Search for an account by account number
    void newaccount(); // Create a new bank account
    void deposit(); // Deposit money into an account
    void withdraw(); // Withdraw money from an account
    void check_account(); // Display account details
    void modifyaccount(); // Modify account information
    void deleteaccount(); // Delete an account
    
    // Constructor to initialize account attributes
    bankmanagement()
    {
        accno=0;
        name="";
        address="";
        actype='\0';
        amount=0.0; 
    }
     
};
