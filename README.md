<h1>Algorithms and data structures Project</h1>
<h2>Development of an algorithm - matrix</h2>
<h2>Description</h2>


There is a real square matrix A of order M. Find a real square matrix B of order N.
matrix B of order N, each of its elements is equal to the sum of the elements of matrix A in the corresponding shaded region defined by the indices i, j:
<img width="281" alt="Снимок экрана 2023-02-20 в 22 04 10" src="https://user-images.githubusercontent.com/87941256/220204972-203fab73-9dcf-4abc-bed9-e2dc9bc3e8c4.png">

<br />
<h2>Algorithm Description</h2>

1) Enter the array A [][] of size N*N <br />
2) Set the values S=0,i=0,j=0<br />
3) Check j<N (if false, go to step 9))<br />
4) Check i<N (if false, increase j++ and return to step 3)
5) Assign p to the value of j and m to the value of i
6) Check m<N (if false, assign b[i][j] the value S, S=0, and return to 4))
7) Check p<N (if false, increase m++ and return to 6)) 8) Increment S by a[m][p] and return to 7)
9) Print the array B[][]

<br />

<h2>Block diagram of the algorithm:</h2>
<img width="597" alt="Снимок экрана 2023-02-20 в 22 01 09" src="https://user-images.githubusercontent.com/87941256/220204694-007c59bf-9822-463c-ada0-db00f0874479.png">

<h2>Algorithm action diagram:</h2>
<img width="348" alt="Снимок экрана 2023-02-20 в 22 03 42" src="https://user-images.githubusercontent.com/87941256/220204932-fcfeac30-35df-4315-8ecb-10aa3c78bff3.png">
