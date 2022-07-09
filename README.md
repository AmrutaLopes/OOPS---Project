# OOPS---Project
Creates a Saving account with methods to update the balance of a customer after deposit &amp; withdrawal(Using OOPS concepts))


# Programming Refresher -  Programming – Course-End Project (Banking Domain)


1.Program begins with Parent class Bank with the corresponding attributes initialization.
  IFSC_Code, BankName, BranchName, loc

2.Next class defined as Customer to initalize customer attributes.
  CustomerID, name, address and contactdetails

3.Account class inherits from Bank class with use of super() method to access / refer to attributes of Bank class.
  Further, it defines 3 methods or functionalities of the same class
  a. getAccountInfo() : gets all the details of Bank class while using Cust object of customer class to access
     information of customer class.
  
  b.deposit(): Prints the vaialbe balance before deposit. It takes the amount parameter passed in deposit method
    when called fetches the corresponding value to be deposited and updates the balance and prints out the message.
  
  c.withdraw() : Prints the available balance. The amount parameter passed in withdraw method getches the value 
    passed when function called. Further it validates if the amount to be withdrawan is 0 or negative amount entered
    and prompts the relevant message. Further it also validates if the amount to be withdrawn is more than balance
    avaialable in the account, if condition satisfies it performs the operation and prints out the message or it condition
    is evaluated to be false it prints out the relevant message.
    
  d.getBalance(): Prints out the updated balance for operations perfomed.

4.SavingsAccount class inherits account class and initializes attribute using super(). It defines and initializes it's own
  class attribute SMinBalance setting it's value.Further it defines it's own methods of getAccountInfo(): whicg returns
  the Savings Account Information, deposit(): which deposits the amount passed in the function and updates the message accordingly.
  withdraw(): which validates the amount to be withdrawn against available balance and also checks for SMinBalance,
  using If-else construct, if condition evaluates to be true it withdraws the amount specified and updates the balance
  while flashing an update message, if condition evaluates to be false a warning message is prompted.


5.Driver Code:  
  Consists of various objects of respective classes.
  5.a) cust1: object of Customer class is instantiated.
  5.b) acc1: object of Account class is instantiated and corresponding methods of Account class using this objects
       have been invoked to perorm the operaions.
  5.c) cust2: another object of Customer class is instantiated.
  5.d) sav1: object of SavingsAccount class is instantiated to perform the operations on the methods of class Savings Account.
