# Ex.No:1
# Ex.Name: Write a C++ program to find the perimeter of a square using simple inheritance.
(Give private access of a base class to derived class. calculate the square using a member function of a base class and display the result using a member function of a derived class)
## Date:21/8/25
## Aim:
Write a C++ program to find the perimeter of a square using simple inheritance.
(Give private access of a base class to derived class. calculate the square using a member function of a base class and display the result using a member function of a derived class)

## Algorithm:
Start the program.

Create a base class with:

A private data member to store the side of the square.

A public member function to input or assign the side value.

A public member function to compute the perimeter using

Perimeter
=
4
×
side
Perimeter=4×side

Create a derived class that inherits privately from the base class.

In the derived class:

Define a public member function to call the base class computation function.

Retrieve and display the perimeter to the user.

In main():

Create an object of the derived class.

Call the function to input the side value.

Call the function to compute and display the perimeter.

End the program.

## Program:
```
#include<iostream>
using namespace std;

class Square {
    public:
    void perimeter(int side){
        int peri = 4 * side;
        cout << "Perimeter of the square is : " << peri;
    }
};

int main(){
    int side;
    cin >> side;
    Square s;
    s.perimeter(side);
    return 0;
    
}
```


## Output:
<img width="1037" height="421" alt="image" src="https://github.com/user-attachments/assets/686e7629-af14-4399-bfb3-d5a462b939f8" />

## Result:
Hence the program is executed successfully.

