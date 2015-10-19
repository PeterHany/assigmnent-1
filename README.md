Name: Peter Hany Alfy
Section: 1
Assignment 1
•	Chapter review:

(1)	What is a Class?
Ans.: A class is a C++ vehicle for translating an abstraction to a user-defined type. It combines data representation and methods for manipulating that data into one neat package.
(2)	How does a class accomplish abstraction, encapsulation, and data hiding?
Ans.: The class accomplish abstraction by giving each part a well-defined interface so that all the other parts and drivers can be able to use it, and it can accomplish encapsulation by making each part well isolated from other parts that it only knows what it has to do and nothing more, and did the data hiding by adding the protected and private parts in the classes so their data are always hidden from users.
(3)	What is the relationship between an object and a class?
Ans.: A class is a definition of the behavior of an object and objects are instances of classes.


(4)	In what way, aside from being functions, are class function members different from class data members?
Ans.: A static variable is a single memory location associated with the class.
A non-static variable (that is a member of a class) represents a different memory location for each instance of the class.
Static variables can be initialized only once and assign to 0 when an object is created.
(5)	Define a class to represent a bank account. Data members should include the depositor’s name, the account number (use a string), and the balance.
Ans.:
#include <iostream>
#include <string>
using namespace std;
class bank_account
{
Private:
String depositor_name , account_number, double balance;
Public:
Void show(string name, string number , double balance);
void withdraw(double balance, double amount);
Void deposit(double balance , double amount);
};

(6)	When are class constructors called? When are class destructors called?
Ans.: Constructors are like "init functions". Minimally they initialize internally used fields. They may also allocate resources (memory, files, semaphores, sockets, etc). 
Class constructor name is the same as class name.
Constructor does not return value but also is not declared type “void”. 
(7)	Provide code for a constructor for the bank account class from Chapter Review Question 5.
Ans.: 
bank_account::bank_account(const std::string & client,
const std::string & num, double bal)
{
Depositor_name = client;
account_number = num;
balance = bal;
}

(8)	What is a default constructor? What is the advantage of having one?
Ans.: A default constructor is a constructor that is used to create an object when you don’t provide explicit initialization values and is called with no arguments.


(9)	Modify the Stock class definition (the version in stock20.h) so that it has member functions that return the values of the individual data members. Note: A member that returns the company name should not provide a weapon for altering the array. That is, it can’t simply return a string reference. It could return a const reference
Ans.:

(10)	What are this and *this?
Ans.: The “this” pointer is available to class methods. It points to the object used to invoke the method. Thus, “this” is the address of the object, and “*this” represents the object itself.

