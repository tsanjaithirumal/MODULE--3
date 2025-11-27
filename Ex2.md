# Ex.No:2
# Ex.Name:Write a C++ program to modulo operation using inheritance (declare two input variable as protected in base class and read one value in one derived class and read another value its derived class and do the modulo operation in its derived class).
## Date:21/8/25
## Aim:
Write a C++ program to modulo operation using inheritance (declare two input variable as protected in base class and read one value in one derived class and read another value its derived class and do the modulo operation in its derived class).


## Algorithm:
Start the program.

Create a base class with:

Two protected data members to store the input values.

Create the first derived class (Derived1) that inherits from the base class:

Define a public method to read the first value and store it in the protected variable.

Create the second derived class (Derived2) that inherits from Derived1:

Define a public method to read the second value and store it in the second protected variable.

Define another public method to perform the modulo operation:

result
=
value1
%
value2
result=value1%value2

Display the result.

In main():

Create an object of the second derived class.

Call the method to read the first value.

Call the method to read the second value.

Call the method to perform and display the modulo operation.

End the program.


## Program:
```
#include <iostream>
using namespace std;
class Base {
      protected:
      int a,b;
      public:
       void read()
      {
          cin>>a;
      }
};
class derived1:public Base
{
    public:
     void sread()
     {
         cin>>b;
     }
     
};
class derived2:public derived1
{
    public:
    void divi()
     {
         cout<<"The Result is:"<<a%b;
     }
};
int main()
{
   derived2 d;
   d.Base::read();
   d.sread();
   d.divi();
}
```


## Output:
<img width="1031" height="423" alt="image" src="https://github.com/user-attachments/assets/5e23043b-8109-446d-ba05-49c303d26e7f" />




## Result:
Hence the program is executed successfully.

