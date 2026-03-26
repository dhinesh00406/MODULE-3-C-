# Ex.No:3
# Ex.Name: Write a C++ program to get two numbers from two base classes and display the quotient in the derived class.
(Illustrate multiple Inheritance and use appropriate access specifier)
## Date:
## Aim:
To write a c++ program to find difference & quotient of two numbers using Hierarchical inheritance

## Algorithm:
1. Start the program.
2. Create a base class with two integer members and a function to read values.
3. Derive a class Difference from the base class and add a function to calculate a - b.
4. Derive another class Quotient from the base class and add a function to calculate a / b.
5. In main(), create objects of derived classes.
6. Call the base class function to input numbers.
7. Call the respective functions to display difference and quotient.
8. End the program.




## Program:
```
#include<iostream>
using namespace std;
class Base
{
    public:
    int a,b;
};
class Derived1:public Base
{
    public:
    void product()
    {
        cin>>a>>b;
        cout<<"Difference="<<a-b<<endl;
    }
};
class Derived2:public Base
{
    public:
    void Sum()
    {
        cin>>a>>b;
        cout<<"Quotient="<<a/b<<endl;
    }
};
int main()
{
    Derived1 d1;
    d1.product();
    Derived2 d2;
    d2.Sum();
    return 0;
}
```



## Output:
<img width="793" height="330" alt="489170559-f6469beb-44b5-483f-9fdd-980228b9f838" src="https://github.com/user-attachments/assets/06b1714a-4f91-4e6c-a1e5-585d9ea57834" />



## Result:
The program successfully executed for difference & quotient of two numbers using Hierarchical inheritance.
