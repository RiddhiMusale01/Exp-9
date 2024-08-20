# EXPERIMENT 9
# Aim
To study and implement C++Pointer basics
# Software Used
Visual Studio Code
# Theory

Pointers are symbolic representations of addresses.
They allow programs to stimulate call-by-preference while also creating and manipulating dynamic data structures.
One of the most common uses for pointers is to iterate over elements in arrays or other data structures.
The address of the variable being worked on is assigned to a pointer variable that points to the same data type.

The reason we associate data type with a pointer is that it knows how many bytes the data contains. When we increment a pointer, we increase it by the size of the data type to which it refers.

Syntax:
```
datatype *var_name;
int *ptr; //ptr can point to an address which holds in data
```

CODES: 

1.Illustrate Pointers:

```
#include <bits/stdc++.h> 
using namespace std;
void geeks()
{
    int var = 5;
    int* ptr;                  
    ptr = &var;

    cout<<"Value at ptr = "<<ptr<<"\n";
    cout<<"Value at var = " <<var<<"\n";
    cout<<"Value at *ptr = "<<*ptr<<"\n";

}

int main()
{
    geeks();
    return 0;
}
```
O/P:

![image](https://github.com/user-attachments/assets/a68de84c-d3e1-4c2e-a93b-7c9953a6cf2e)

2. 1D Array of pointers:
```
#include <iostream> 
using namespace std; 

int main() 
{
    int* p=new int[7];  

    for (int i=0; i<5; i++)  
    {
        p[i]=10*(i+1);
    }

    cout<<*p<<"\n"; 
    cout<<*p+1<<"\n";
    cout<<*(p+1)<<"\n";
    cout<<2[p]<<"\n";
    cout<<p[2]<<"\n";
    *p++;

    cout<<*p;                

    return 0; 
}
```
O/P:

![image](https://github.com/user-attachments/assets/bc970f1c-8aab-45bb-a7d1-b86af1684798)

# Conclusion 
Both codes are foundational in understanding how memory management and pointer arithmetic work in C++. They show the power and potential pitfalls (like pointer manipulation) of using pointers.
