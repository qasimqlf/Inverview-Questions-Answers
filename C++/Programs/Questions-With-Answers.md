## C++


#### Q1. Write a program to print Even Numbers from 1 to 100?

```cpp
#include <iostream>
using namespace std;

int main() {
 
    int i;
 
    /* Run a loop from 1 to 100. */
 
    for(i = 1; i < = 100; i++){
  
       /* If number is divisible by 2. */
  
      if(i % 2 == 0) {

         cout << i <<" "; 
      }
   }
    return 0;
}
```

#### Q2. Fibbonacci series by using recursion?

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

#### Q3. Write a program to convert normal case to camel case

```cpp
#include <iostream>
#include <string>

int main()
{
    int count;

    std::cout << "Enter film count: ";
    std::cin >> count;
    if(std::cin.fail())
    {
        std::cout << "Invalid input." << std::endl;
        exit(0);
    }
    std::cin.ignore(10000,'\n');
    for(int i = 0; i < count; i++)
    {
        std::string film;
        std::cout << "Enter film name: ";
        std::getline(std::cin, film);
        if(std::cin.fail())
        {
            std::cout << "Invalid input." << std::endl;
            exit(0);
        }
        if(film.size() == 0)
            break;
        film[0] = tolower(film[0]);
        for(unsigned int i = 1; i < film.size() - 1; i++)
        {
            if(film[i] == ' ')
            {
                film.erase(i,1);
                film[i] = toupper(film[i]);
                i--;
            }
        }
        std::cout << "Result: " << film << std::endl;
     }

    return 0;
}
```
