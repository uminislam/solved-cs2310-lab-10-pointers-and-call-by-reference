Download Link: https://assignmentchef.com/product/solved-cs2310-lab-10-pointers-and-call-by-reference
<br>
<strong>Q-1.</strong> Write a program that asks the user to enter integers as inputs to be stored in the variables <strong>A</strong> and <strong>B</strong> respectively. There are also two integer pointers named <strong>ptrA</strong> and <strong>ptrB</strong>. Assign the addresses of <strong>A</strong> and <strong>B</strong> to <strong>ptrA</strong> and <strong>ptrB</strong> respectively and display the values in <strong>A</strong> and <strong>B</strong> using <strong>ptrA</strong> and <strong>ptrB</strong>.

<strong>Note</strong>:

<ul>

 <li>Outputs may be different in different runs as we print addresses in program, the same hereinafter.</li>

 <li>To manipulate the stream to print foo in hexadecimal use the hex manipulator: cout &lt;&lt; hex &lt;&lt; foo;</li>

</ul>




<strong><u>Expected Outputs:</u></strong>

Enter value of A: <u>10</u>

Enter value of B: <u>20</u>

Value of ptrA is 10 stored in address 002EF83C

Value of ptrB is 20 stored in address 002EF830










<ul>

 <li>Write a C++ program to find the max of an integer array. The program will ask the user to input the size of the array and the value of each element. The program prints on screen the maximum value in this array and the pointer that points to the maximum value.</li>

</ul>

<strong><u>Expected Outputs.</u></strong>

<table width="0">

 <tbody>

  <tr>

   <td width="552">Enter number of values: <u>3</u> Enter values in array:1 2 3Largest integer value in the array is 3Largest integer value in the array is stored in address00659AC8</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong> </strong>







<strong> </strong>

1




<em>Computer Programming</em>

<ul>

 <li>Download ex1.cpp and ex2.cpp. Compile and execute the program. Explain the output.</li>

</ul>

<table width="0">

 <tbody>

  <tr>

   <td width="108"><strong><em>File</em></strong></td>

   <td width="459"><strong><em>Program segment</em></strong></td>

  </tr>

  <tr>

   <td width="108">Ex1.cpp</td>

   <td width="459">#include <strong>&lt;iostream&gt; </strong><strong> </strong><strong>using namespace </strong>std; <strong>int </strong>main() {     <strong>int </strong>v = 5, *ptr;     ptr = &amp;v;     *ptr = 42;cout &lt;&lt; <strong>“v = ” </strong>&lt;&lt; v &lt;&lt; endl;     cin &gt;&gt; *ptr; <em>// Let’s enter 100 </em><em>    // What happens if you write cin &gt;&gt; ptr; ?     </em>cout &lt;&lt; <strong>“v = ” </strong>&lt;&lt; v &lt;&lt; endl;     v = 7;cout &lt;&lt; <strong>“*ptr is ” </strong>&lt;&lt; *ptr &lt;&lt; endl;     cout &lt;&lt; <strong>“Address of v is ” </strong>&lt;&lt; ptr &lt;&lt; endl;     <strong>return </strong>0;} </td>

  </tr>

  <tr>

   <td width="108">Ex2.cpp</td>

   <td width="459">#include <strong>&lt;iostream&gt; </strong><strong> </strong><strong>using namespace </strong>std; <strong>void </strong>f(<strong>int </strong>*a, <strong>int </strong>*b) {<strong>int </strong>*c;     c = a;     *c = *c + 10;*b = *b + 10;}<strong>int </strong>main() {     <strong>int </strong>x = 3, y = 4;     <strong>int </strong>*ptr1;     ptr1 = &amp;x;     f(ptr1, &amp;y);cout &lt;&lt; <strong>“x = ” </strong>&lt;&lt; x &lt;&lt; endl;     cout &lt;&lt; <strong>“y = ” </strong>&lt;&lt; y &lt;&lt; endl;     cout &lt;&lt; <strong>“*ptr1 = ” </strong>&lt;&lt; *ptr1 &lt;&lt; endl;     <strong>return </strong>0;} </td>

  </tr>

 </tbody>

</table>










2


