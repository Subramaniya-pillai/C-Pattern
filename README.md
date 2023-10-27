# Pattern

## Aim:
To Write a C# program for pascal triangle.
## Equipment Required:
Microsoft Visual Studio 2022.
## Algorithm:
### Step1:
Start the program. 
### Step2:
Get the limit from the user. 
### Step3:
Use for loop to print the rows , columns and space. 
### Step4:
Use if-else condition inside the loop to print the values. 
### Step5:
Use c = c * (i - j + 1) / j to print the inner value. 
### Step6:
Using Console.write print the Pascal's triangle. 
### Step7:
End the program.
## Program:

>Developed By: Subramaniya PIllai B

>Reg No: 212221230109

```
using System;
namespace ex3
{
    class Program
    {
        public static void Main(string[] args)
        {
            int rows = 6, val = 1, blank, i, j;
            Console.WriteLine("Pascal's Triangle");
            for(i=0; i<rows; i++) 
            {
                for (blank = 1; blank <= rows - i; blank++)
                    Console.Write(" ");
                for (j = 0; j <= i; j++)
                {
                    if (j == 0 || i == 0)
                        val = 1;
                    else
                        val = val * (i - j + 1) / j;
                    Console.Write(val + " ");                    
                }
                Console.WriteLine();
            }

        }
    }
}
```
## Output:

![Alt text](o1.jpg)

## Result:
Thus, C# program for a pascal's triangle is executed successfully.
