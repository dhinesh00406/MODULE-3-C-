# Ex.No:1
# Ex.Name: Write a c++ program to find simple & compound interest by using Hierarchical Inheritance (read the data In the order of p, n & r)
## Date:
## Aim:
To wite a c++ program to find simple & compound interest by using Hierarchical Inheritance (read the data In the order of p, n & r)



## Algorithm:
1. Start the program.
2. Create a base class to store principal, time, and rate with input function.
3. Derive SimpleInterest class to calculate (p * n * r) / 100.
4. Derive CompoundInterest class to calculate p * (pow((1 + r/100), n) - 1).
5. In main(), create objects of derived classes.
6. Call input function once from base class.
7. Calculate and display SI and CI.
8. End the program.




## Program:
```
#include <iostream>  
#include<cmath>
using namespace std;  
  
int main()
{
    float p,n,r,k;
    cin>>p>>n>>r;
    cout<<"Simple Interest Amount is :="<<p*n*r/100<<endl;
    k=p*pow((1+r/100),n)-p;
    cout<<"Compound Interest Amount is :="<<k;
}
```


## Output:

<img width="1124" height="382" alt="566359640-c5915f2a-cc3b-487f-9e93-33ff043672c8" src="https://github.com/user-attachments/assets/d4994454-db8e-4b79-9558-e00d745e8e1d" />



## Result:
The program successfully executed for simple & compound interest by using Hierarchical Inheritance.
