# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list<br>
Developed by:sanjay sivaramakrishnan M<br>
RegisterNumber: 23013798<br>
'''<br>
def linearseach():<br>
    arra=eval(input())<br>
    arra.sort()<br>
    print(arra)<br>
    find=int(input())<br>
    check=0<br>
    index=0<br>
    sum=0<br>
    for i in arra:<br>
        if(i==find):<br>
            index=sum<br>
            check=1<br>
            break<br>
        sum+=1<br>
            <br>
    if(check==1):<br>
        print(f"Element found at index:  {index}")<br>
    else:<br>
        print("Element not found")<br>
        <br>
linearseach()<br>
<br>


```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```






```
iii)	# Find the element in a list using Binary Search (recursive Method).
```





```
## Sample Input and Output
![image](https://github.com/sanjaysivaramakrishnan/Search-Algorithm/assets/151629616/249278c6-8cad-4350-b24f-71991e3aea01)






## Result
Thus the linear search and binary search algorithm is implemented using python programming.
