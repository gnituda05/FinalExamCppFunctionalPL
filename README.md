# FinalExamCppFunctionalPL

Problem: Suppose we have 30 students each studying 2 subjects (subject 1 and subject 2) and we have to display the marks in both the subjects of the 30 students.  30 students studied only 2 subjects. <br />
*PS in this problem I will input the marks from student but only 3 students will be ouputed for this Syntax for that we can easily see the marks of rach student when it comes to mass of population. <br />

**In this Problem I use 2D arrays for the list.**<br />
Why if arrays are  2D? <br />
 -  2-dimensional arrays also exist and are generally known as matrix. These consist of rows and columns.
Before going into its application, let's first see how to declare and initialize a 2 D array.
Similar to one-dimensional array, we define 2-dimensional array as below.


![image](https://user-images.githubusercontent.com/70184357/159165641-53dd33d6-508b-40d3-b2a0-ae5fd90dcfa8.png)<br />
Here, a is a 2-D array of type int which consists of 2 rows and 4 columns. <br />
It is like: <br />
        Column 0 || Column 1 || Column 2 || Column 3
Row 0   a[0][0]     a[0][0]      a[0][0]    a[0][0] 
Row 1   a[1][0]     a[1][1]      a[1][2]    a[1][3] 

Now let's see how to initialize a 2-dimensional array.
**Initialization of 2 D Array**
Same as in one-dimensional array, we can assign values to a 2-dimensional array in 2 ways as well.
In the first method, just assign a value to the elements of the array. If no value is assigned to any element, then its value is assigned zero by default.
Suppose we declared a 2-dimensional array a[2][2]. Then to assign it values, we need to assign a value to its elements.
int a[2][2];
a[0][0]=1;
a[0][1]=2;
a[1][0]=3;
a[1][1]=4;

The second way is to declare and assign values at the same time as we did in one-dimensional array.
int a[2][3] = { 1, 2, 3, 4, 5, 6 };

Here, value of a[0][0] is 1, a[0][1] is 2, a[0][2] is 3, a[1][0] is 4, a[1][1] is 5 and a[1][2] is 6.
We can also write the above code as:
int a[2][3] = {
    {1, 2, 3},
    {4, 5, 6 }
};
Let's consider different cases of initializing an array.
int a[2][2] = { 1, 2, 3, 4 }; /* valid */
int a[ ][2] = { 1, 2, 3, 4 }; /* valid */
int a[2][ ] = { 1, 2, 3, 4 }; /* invalid */
int a[ ][ ] = { 1, 2, 3, 4 }; /* invalid */

As we understand the flow of the 2D we'll understand the problem too.
This link using 'Mycompiler' you will see the code itself of the problem
** https://www.mycompiler.io/view/8vboItAYjoz **

In the above example, firstly we defined our array consisting of 3 rows and 2 columns as float marks[3][2];
Here, the elements of the array will contain the marks of the 3 students in the 2 subjects as follows.

![image](https://user-images.githubusercontent.com/70184357/159165971-2c9d6974-8e20-4ef0-bf6c-f07bcb10942e.png)

In our example, firstly we are taking the value of each element of the array using a for loop inside another for loop.
In the first iteration of the outer for loop, value of 'i' is 0. With the value of 'i' as 0, when the inner for loop first iterates, the value of 'j' becomes zero and thus marks[i][j] becomes marks[0][0]. By writing cin >> marks[i][j];, we are taking the value of marks[0][0].

After that, the inner for loop again iterates and the value of 'j' becomes 1. marks[i][j] becomes marks[0][1] and its value is taken from the user.

Then, the outer loop iterates for the second time and the value of 'i' becomes 1 and the whole process continues.

After assigning the values to the elements of the array, we are printing the values of the elements of the array, in the same way, using another for loop inside for loop.
















