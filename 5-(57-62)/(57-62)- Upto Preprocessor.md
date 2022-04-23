## Lec 57 - (Lecture 17 union in C Language Part 1)

What is union?

- Union is similar to structure, except it allows you to define variables that share storage space

- Defining union means creating new data type



**struct Vs union:**

<img src="./images/1.png" title="" alt="" width="428">



i1 in <u>union</u> gets only that much  memory that the maximum memory taken by float y i.e. 4 bytes

so, item type variable gets 4 bytes memory... 



Example:

<img src="./images/2.png" title="" alt="" width="458">

```c
#include <stdio.h>

union Item{
    int x;
    float y;
    char z;
};
int main(){
   
   union Item i1;
   i1.x=2;
   printf("x = %d\n",i1.x);
   
   i1.y=3.5;
   printf("y = %f\n",i1.y);
   
   i1.z='a';
   printf("z = %c\n",i1.z);
   
   return 0;
}
```

Disscussion:

<img title="" src="./images/3.png" alt="" width="550">

At particular time we can print / do only one thing...



**How to access?**

- Union members are accessed in the same manner as we access structure member

---------

## Lec 58 - (Lecture 19 Enumerators in C Language)


