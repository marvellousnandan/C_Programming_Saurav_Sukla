# Introduction To C

<img src="./Images/1.png" title="" alt="" width="471">

## Hello World

```c
#include <stdio.h>
int main() {
    printf("Hello World!");
}
```

This is Hello World Program

-----------------------------------------------------------------------------

*Notes From Lec 1 -11 on Copy*

----------------------------------------------------------------------------------------

## Lec 12 - Arithmetic Instruction in C(Part -1 )

**NOTE:** There is no BODMAS in "C" language

-------------------

## Lec 13 (P-2)

**OPERATOR GROUPS:**

- Unary Operators

- Arithmetic Operators

- Bitwise Operators

- Relational Operators

- Logical Operators

- Conditional Operator

- Assignment Operators

**UNARY OPERATORS:**

Here Only one operand is required

- +,-,++,--,sizeof()

        Binary Operator:  Operators required two operands...    

        TERNIARY OPERATOR: Operators required Three operands

// Use of x++, ++x

```c
// ++ increment operator
main()
{
int x=3;
clrscr();
x++; //x=x+1 Post increment
printf("%d",x);
++x; //x=x+1 Pre increment
printf("%d",x);
getch();
}
```

// Use of  x-- , --x

```c
// -- decrement operator
main()
{
int x=3;
clrscr();
x--; //x=x-1  Post decrement
printf("%d",x);
--x; //x=x-1  Pre decrement
printf("%d",x);
getch();
}
```

## Lec 14 (P-3)

**sizeof()**: It's an operator which tells the size (Unit: bytes)

- sizeof(data type)

- sizeof(variable)

- sizeof(constant)

e.g.: Size of float => 4 bytes

```c
// sizeof()
main()
{
int x;
clrscr();
x=sizeof(float);
// x=sizeof(double);
// x=sizeof(char);
// x=sizeof(int);
printf("%d",x);
getch();
}
```

```c
// Sizeof()
main()
{
int x,y;
float k;
double d1;
char ch;
clrscr();
x=sizeof(ch);
// x=sizeof(y);
// x=sizeof(d1);
// x=sizeof(k);

printf("%d",x);
getch();
}
```

```c
// sizeof()
main()
{

int x,y,z;
clrscr();
x=sizeof(34);
y=sizeof(3.56);
z=sizeof(‘a');
printf("%d %d %d",x,y,z);
getch();
}
```

```c
// sizeof() (CORRECT ONE)
#include <stdio.h>
main()
{

int x,y,z;

x=sizeof(34);   //34 -> Integer
y=sizeof(3.56); //3.56 -> Real constants are type of "double"

z=sizeof('a'); 
/*
ASCII, a -> 97
a -> Character
z=sizeof(97); //97 -> Integer
*/
printf("%d %d %d",x,y,z);
}
```

---------------------------------------

## Lec 15

**ARITHEMATIC OPERATORS:**

->     *    /    % 

->       +     -

Associativity Rule Left to Right

```c
// Use of Divide Operator

main()
{
int x;
x=3.0/4;
printf("%d",x);
}

/*
3/4         0
3.0/4       0.75
3/4.0       0.75
3.0/4.0     0.75
*/
```

```c
main()
{
int x;
x = 25%5;
// x = 3/4;
// x = 13/4;
printf("%d",x);
}
```

NOTE: Whenever we need to check whether number is divisible or not from a number use Module operator(%) instead of divide operator(/). 

----------------------------------

## Lec 16

**<u>BITWISE OPERATORS:</u>**

Bitwise AND        &
Bitwise OR           |
Bitwise XOR         ^
Bitwise NOT         ~
Right Shift            >>
Left Shift              <<

<u>**& Operator**</u>

- 0 & 0 = 0

- 0 & 1 = 0

- 1 & 0 = 0

- 1 & 1 = 1

Note: 0,1 are operands of Bitwise Operator

<img title="" src="./Images/2.png" alt="2.png" width="522">

**<u>| Operator</u>**

- 0 | 0 = 0

- 0 | 1 = 1

- 1 | 0 = 1

- 1 | 1 = 1

<img title="" src="./Images/3.png" alt="3.png" width="560">

**<u>^ Operator</u>**

- 0 ^ 0 = 0

- 0 ^ 1 = 1

- 1 ^ 0 = 1

- 1 ^ 1 = 0

![](./Images/4.png)

**<u>Right Shift</u>**

<img title="" src="./Images/5.png" alt="5.png" width="574">

**<u>Left Shift</u>**

<img title="" src="./Images/6.png" alt="6.png" width="588">

-----------
