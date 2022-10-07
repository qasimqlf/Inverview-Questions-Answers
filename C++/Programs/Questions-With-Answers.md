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
