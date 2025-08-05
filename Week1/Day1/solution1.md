

## What's the Question?

We have a simple C function that takes two numbers and does something with them. Let's see what happens when we give it `a = 6` and `b = 1`.

The function is supposed to:
- Double the first number (a)
- Double the second number (b)  
- Add them together and give us the answer

## Let's Think Through It Step by Step

**Starting with:** a = 6, b = 1

**Step 1:** Double the value of a
- a was 6
- a + a = 6 + 6 = 12
- Now a = 12

**Step 2:** Double the value of b  
- b was 1
- b + b = 1 + 1 = 2
- Now b = 2

**Step 3:** Add them together
- a + b = 12 + 2 = 14

**Answer:** 14

## The C Code

Here's what the actual code looks like:

```c
#include <stdio.h>

int funn(int a, int b) {
    a = a + a;  // 6 becomes 12
    b = b + b;  // 1 becomes 2
    return a + b;  // 12 + 2 = 14
}

int main() {
    int result = funn(6, 1);
    printf("%d\n", result);
    return 0;
}
```

## What Happens When We Run It?

The program will print: **14**

## Why Does This Work?

Think of it like this:
- You have 6 apples, you get 6 more → now you have 12 apples
- You have 1 orange, you get 1 more → now you have 2 oranges  
- Total fruit = 12 + 2 = 14 pieces of fruit

## Let's Try Other Examples

- If a = 3 and b = 4:
  - Double 3 → 6
  - Double 4 → 8  
  - Answer: 6 + 8 = 14

- If a = 0 and b = 5:
  - Double 0 → 0
  - Double 5 → 10
  - Answer: 0 + 10 = 10

- If a = 2 and b = 2:
  - Double 2 → 4
  - Double 2 → 4
  - Answer: 4 + 4 = 8

## The Simple Answer

When we put a = 6 and b = 1 into our function, we get **14** as the output.

That's it! Pretty simple, right?
