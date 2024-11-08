# Ex.No: 6 SORTING
## DATE:
## REGISTER NUMBER : 212222040037
### AIM:
Write a Python program for sorting and inspect for failures.

### Algorithm:
1. Start the program.
2. Get the number of elements from user
3. Get the elements to be sorted
4. Traverse the array and sort the elements one by one
5. Print the sorted array
6. Stop the program.
   
### Program:
```
n = int(input("Enter the number of elements: "))
arr = []
try:
    for i in range(n):
        a = float(input("Enter the element: "))
        arr.append(a)
    
    # Sorting the array using Bubble Sort
    for i in range(n):
        for j in range(i + 1, n):
            if arr[i] > arr[j]:
                temp = arr[i]
                arr[i] = arr[j]
                arr[j] = temp

    print("The array after sorting:")
    for i in range(n):
        print(int(arr[i]), end=' ')
        
except ValueError:
    print("Enter a valid number")
```
### Output:
![sorting output](https://github.com/user-attachments/assets/d2765b87-6b1f-41f5-8bdd-324d0c328343)


### Result:
Thus, a program for sorting has been written and test cases have been written and verified successfully.
