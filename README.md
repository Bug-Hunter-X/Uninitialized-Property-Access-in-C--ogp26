# Uninitialized Property Access in C#

This example showcases a common error in C#: accessing a property before it has been explicitly assigned a value.  In C#, class members are initialized to their default values (0 for integers, null for references, etc.) if no explicit initialization is provided. Accessing a property before assigning a value might lead to unexpected behavior or runtime errors depending on the context.

## How to Reproduce
1. Compile and run the provided code (bug.cs).
2. Observe the output. The value printed might be 0, but this is not always guaranteed and can change based on the C# compiler and runtime environment.

## Solution
The solution (bugSolution.cs) demonstrates initializing the property before accessing it to prevent undefined behavior.
