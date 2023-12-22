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
''' 
Program to find the element in a list using Binary Search(Iterative Method)..<br>
Developed by: Sanjay siavaramakrishnan M<br>
RegisterNumber: 23013798<br>
'''<br>
def binarySearchIter(array,l,u,find):<br>
    while l<=u:<br>
        mid=l+(u-l)//2<br>
        if(array[mid]==find):<br>
            return mid<br>
        elif(array[mid]<find):<br>
            l=mid+1<br>
        else:<br>
            u=mid-1<br>
    return 0<br>        
array=eval(input())<br>
array.sort()<br>
u=len(array)-1<br>
f=int(input())<br>
x=binarySearchIter(array,0,u,f)<br>
print(array)<br>
if(x==0):<br>
    print("Element not found")<br>
else:<br>
    print(f"Element found at index:  {x}")<br>
     <br>

```
iii)	# Find the element in a list using Binary Search (recursive Method).
```

''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: Sanjay sivaramakrishnan M
RegisterNumber: 23013798
'''
def BinarySearch(array, find, l,u):<br>
  if l<=u:    <br>
    mid=l+(u-l)//2<br>
    if(array[mid]==find):<br>
        return mid<br>
    elif(array[mid]<find):<br>
        l=mid+1<br>
        return BinarySearch(array, find, l,u)<br>
    else:<br>
        u=mid-1<br>
        return BinarySearch(array, find, l,u)<br>
   <br>
  return -1<br>
    <br>
arr = eval(input())<br>
arr.sort()<br>
k = eval(input())<br> 
l=0<br>
h=len(arr)-1<br>
x=BinarySearch(arr, k, l, h)<br>
print(arr)<br>
if(x==-1):<br>
    print("Element not found")<br>
else:<br>
    print(f"Element found at index:  {x}")<br>
<br>


```
## Sample Input and Output
![image](https://github.com/sanjaysivaramakrishnan/Search-Algorithm/assets/151629616/249278c6-8cad-4350-b24f-71991e3aea01)
![image](https://github.com/sanjaysivaramakrishnan/Search-Algorithm/assets/151629616/c8d7748d-76fd-47c4-8c95-818516abddb3)
![image](https://github.com/sanjaysivaramakrishnan/Search-Algorithm/assets/151629616/ef85fef1-e11a-4426-9ba9-d3d237434ff0)






## Result
Thus the linear search and binary search algorithm is implemented using python programming.
