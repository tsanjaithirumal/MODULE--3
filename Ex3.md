# Ex.No:3
# Ex.Name: Write a C++ program to illustrate Employee Based Multiple inheritance with protected access specifier, find the income after the payment of tax.. 
( Declare a base class to get salary amount, another base class to get tax amount , declare a salary derived class to call the functions from two base classes and perform calculation)
## Date:21/8/25
## Aim:
Write a C++ program to illustrate Employee Based Multiple inheritance with protected access specifier, find the income after the payment of tax.. 

( Declare a base class to get salary amount, another base class to get tax amount , declare a salary derived class to call the functions from two base classes and perform calculation)


## Algorithm:
Start the program.

Create the first base class (SalaryBase) with:

A protected data member to store the salary amount.

A public method to read the salary.

Create the second base class (TaxBase) with:

A protected data member to store the tax amount.

A public method to read the tax.

Create a derived class (Employee) that inherits protectedly from both base classes.

In the derived class:

Define a public method to access both base class input methods.

Define another public method to calculate the net income using:

Income
=
Salary
−
Tax
Income=Salary−Tax

Display the net income.

In main():

Create an object of the derived class.

Call the method to input salary and tax.

Call the method to compute and display the income.

End the program.





## Program:
```
#include<iostream>
using namespace std;

class IncomeTax {
    public:
    void findTaxedAmount(int principal,int amount){
        cout << "Income after the payment of Tax : " << principal - amount;
    }
};

int main(){
    int principal,amount;
    cin >> principal >> amount;
    IncomeTax tax;
    tax.findTaxedAmount(principal,amount);
    return 0;
}
```


## Output:

<img width="1041" height="521" alt="image" src="https://github.com/user-attachments/assets/1310da30-98b9-40c6-bd63-9f0545dffde4" />




## Result:
Hence the program is executed successfully.

