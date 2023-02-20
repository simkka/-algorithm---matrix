<h1>Algorithms and data structures Project</h1>
<h2>Development of an algorithm - matrix</h2>
<h2>Description</h2>


There is a real square matrix A of order M. Find a real square matrix B of order N.
matrix B of order N, each of its elements is equal to the sum of the elements of matrix A in the corresponding shaded region defined by the indices i, j:<br />

<img width="281" alt="Снимок экрана 2023-02-20 в 22 04 10" src="https://user-images.githubusercontent.com/87941256/220204972-203fab73-9dcf-4abc-bed9-e2dc9bc3e8c4.png"><br />
Here are two algorithms for solving this problem.<br />
<br />
<h2>Algorithm Description №1</h2>

1) Enter the array A [][] of size N*N <br />
2) Set the values S=0,i=0,j=0<br />
3) Check j<N (if false, go to step 9))<br />
4) Check i<N (if false, increase j++ and return to step 3)
5) Assign p to the value of j and m to the value of i
6) Check m<N (if false, assign b[i][j] the value S, S=0, and return to 4))
7) Check p<N (if false, increase m++ and return to 6)) 8) Increment S by a[m][p] and return to 7)
9) Print the array B[][]

<br />

<h2>Algorithm Description №2</h2>
1) Enter the size of the array N;<br />
2) Assign i=0, j=0;<br />
3) Assign to the last element of array B[N-1][N-1] the value<br />
of the last element of array A[N-1][N-1];
4) Calculate the elements of the last line of array B from the end by adding to
the value of the corresponding element of the previous calculated element B
of array A;
5) Similarly, fill the last column of array B;
6) Fill in the remaining elements by adding to the corresponding element A
the value of element B, which is one below, and the value of element B, which is one to the right, and subtract the value of element B, which is one below and to the right (B[i][j]=B[i+1][j]+B[i][j+1]-B[i+1][j+1]+A[i][j]);
7) Print the array B.
<br />

<h2>Block diagram of the algorithm 1:</h2>
<img width="597" alt="Снимок экрана 2023-02-20 в 22 01 09" src="https://user-images.githubusercontent.com/87941256/220204694-007c59bf-9822-463c-ada0-db00f0874479.png">

<h2>Algorithm action diagram 1:</h2>
<img width="348" alt="Снимок экрана 2023-02-20 в 22 03 42" src="https://user-images.githubusercontent.com/87941256/220204932-fcfeac30-35df-4315-8ecb-10aa3c78bff3.png">
 
<h2>Algorithm action diagram 2:</h2>
<img width="387" alt="Снимок экрана 2023-02-20 в 22 35 55" src="https://user-images.githubusercontent.com/87941256/220208023-0002953b-5031-44b3-9980-488184afbe9c.png">

