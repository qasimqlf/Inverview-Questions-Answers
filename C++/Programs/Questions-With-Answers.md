## C++

#### Q1. Fibbonacci series by using recursion?

```cpp
#include<iostream>
using namespace std;

int fbseries(int n)
{

    
    if(n==0)
        return 0;
    
    if(n==1)
     return 1;
 
    
   int ans = fbseries(n-1)+fbseries(n-2);
   return ans;

}

int main()
{
    
    int n;
    cout<<"Enter the term for fibonacci number : "<<endl;
    cin>>n;
    int ans=fbseries(n);
    cout<<endl<<"The fibonacci series term is : "<<ans<<endl;

    return 0;


}

//  Output format :  Enter the term for fibonacci number : 3
//                   The fibonacci series term is : 2
```
