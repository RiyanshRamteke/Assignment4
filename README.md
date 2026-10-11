# Assignment4: References, Pointers, and new/delete in C++

## Problem Statement

a) Write a C++ program based on pointers and references.
b) Write a C++ program using the `new` and `delete` operators for dynamic memory allocation.

Both parts are combined in a single program.

## Objectives

- Understand pointers and references in C++.
- Pass arguments to functions by pointer and by reference.
- Allocate and free memory at run time using `new`, `new[]`, `delete` and `delete[]`.
- Avoid memory leaks and dangling pointers.

## Concepts Used

- **Pointer:** a variable that stores the address of another variable (`int *ptr = &x;`).
- **Reference:** another name (alias) for an existing variable (`int &ref = x;`).
- **new:** allocates memory on the heap at run time.
- **delete / delete[]:** releases memory allocated by `new` / `new[]`.

## Files

| File | Description |
|---|---|
| `main.cpp` | Combined program for pointers, references, and new/delete |
| `README.md` | Project description |

## How to Compile and Run

```bash
g++ main.cpp -o main
./main
```

On Windows (PowerShell):

```powershell
g++ main.cpp -o main
.\main
```

## Sample Output

Input: `n = 3`, numbers `10 20 30`

```
--- Part A: Pointer and Reference ---
x = 10
Value using pointer = 10
Value using reference = 10
x after changing with pointer = 20
x after changing with reference = 30

Before swap: a = 5, b = 9
After swapByPointer: a = 9, b = 5
After swapByReference: a = 5, b = 9

--- Part B: new and delete ---
Dynamic number = 25
Enter how many numbers: 3
Enter 3 numbers: 10 20 30
Numbers are: 10 20 30 
Sum = 60
Memory freed
```

## Test Cases

| Test Case | Input | Expected Output | Status |
|---|---|---|---|
| 1 | n = 3; numbers 10 20 30 | Sum = 60, memory freed | Pass |
| 2 | n = 5; numbers 5 10 15 20 25 | Sum = 75, memory freed | Pass |

## Conclusion

The program demonstrates pointers, references, and call by pointer/reference. It also shows how `new` and `delete` manage dynamic memory, and why every allocation must be freed to prevent memory leaks.

## Tools Used

- Language: C++
- IDE: Visual Studio Code
- Compiler: g++
- Library: iostream
