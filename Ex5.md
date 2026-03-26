# Ex.No:5
# Ex.Name: Write a C++ program to multiply two numbers using  derived constructor.
## Date:
## Aim:
To write a C++ program to display the Employee details using the multiple inheritance constructors.

## Algorithm:
1. Start the program.
2. Create base class EmpID with constructor to set employee ID.
3. Create base class EmpName with constructor to set employee name.
4. Create derived class Employee inheriting from both base classes.
5. In derived class constructor, call both base class constructors and set designation.
6. Add function in derived class to display ID, name, and designation.
7. In main(), get ID, name, and designation from user.
8. Create Employee object with input values.
9. Call display function.
10. End the program.




## Program:
```
#include <iostream>
using namespace std;
class base1
{
    public:
        int eid;
        void get1(){
            cin>>eid;
        }

};
class base2
{
    public:
        string name,desig;
        
        void get2(){
            cin>>name>>desig;
        }
};
class derive1 : public base1, public base2
{
    public:
        void display(){
            cout<<" Employee ID : "<<eid<<endl;
            cout<<" Employee Name : "<<name<<endl;
            cout<<" Employee Designation : "<<desig<<endl;
        }
};
int main ()
{
    derive1 obj;
    obj.get1();
    obj.get2();
    obj.display();
 return 1;   
}
```



## Output:
<img width="1020" height="397" alt="489177834-db355508-f318-4569-acad-7086a8261cbd" src="https://github.com/user-attachments/assets/2b37cec6-9bb7-4026-9026-53680f390455" />



## Result:
The program successfully executed to display the Employee details using the multiple inheritance constructors.
