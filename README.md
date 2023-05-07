# Ex05-Rec-JaggedArray

## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.

## Algorithm:
### Step 1:
Import the 'System' namespace to use the classes present in the 'System' namespace.

### Step 2:
Declare and Initialize jagged Array named cpu with 4 nodes. Array Size is 4.

### Step 3:
Set the size of first array as 3. Set the size of second array as 5. Set the size of third array as 4. Set the size of fourth array as 6.

### Step 4:
Using for loop calculate the cpu usage for each node.

### Step 5:
Compile and Run the Program.


## Program:

```
Developed by: Harini.B
Register Number: 212221230035
```

```
using System;
namespace standard
{
    class Program
    {
        public static void Main(string[] args)
        {
            int[][] cpu = new int[4][];
            cpu[0]=new int[3];
            cpu[1]=new int[5];
            cpu[2]=new int[4];
            cpu[3]=new int[6];
            for(int i=0; i<4; i++)
            {
                for(int j=0; j < cpu[i].Length; j++)
                {
                    cpu[i][j] = i*j+70;
                }
            }
            for(int i=0; i<4;i++)
            {
                for(int j = 0; j < cpu[i].Length; j++)
                {
                    Console.WriteLine("CPU usage for node {0} is {1}", i, cpu[i][j]);
                }
                Console.WriteLine();
            }
        }
    }
}
```


## Output:
![image](https://user-images.githubusercontent.com/93427253/236686486-7c3d5f99-c5ce-4795-9e1d-ecb9d7a03920.png)

## Result:
C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is written and executed.
