# Recursive-function

## Aim: To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step 1: 
Create a class called reverse.

### Step 2: 
Create a recursive function named Revfun to reverse the number

### Step 3: 
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step 4: 
Recusively call this function to get the reversed number.

### Step 5:
Create a Main function

### Step 6:
Get input from the user for the number to be reversed.

### Step 7: 
Call the function Revfun

### Step 8:
End of the program.

## Program:
```
Developed By : Vidya Neela M
Reg No : 212221230120
```
```
using System;
class reverse
{
    public int rev = 0, rem;
    static void Main(string[] args)
    {
        int num;
        Console.Write("Enter the number to reverse: ");
        num = Convert.ToInt32(Console.ReadLine());
        reverse r = new reverse();
        Console.WriteLine("Number after reverse  = " + r.reversefun(num));
        

    }

public int reversefun(int num)
    {
        if (num > 0)
        {
            rem = num % 10;
            rev = rev * 10 + rem;
            return reversefun(num/10);
        }
        return rev;
    }
}

```

## Output:
![image](https://github.com/vidyaneela/Recursive-function/assets/94169318/0b90f768-0ad8-4f20-9c6e-a571b821930a)

## Result:
Thus C# program to reverse a number using recursive function is written and executed sucessfully.
