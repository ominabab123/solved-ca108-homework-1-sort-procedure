Download Link: https://assignmentchef.com/product/solved-ca108-homework-1-sort-procedure
<br>
Part I: Implement a Sort Procedure (P &amp; H, Section 2.12) using QtSPIM.        In class, we introduced MIPS instruction set and showed you an example of sort procedure in instructions. Now we ask you to implement sort procedure using QtSPIM, a MIPS processor simulator which support pseudo-instructions. Repeat the sorting program on page 132 to sort 10 numbers {-1, 3, -5, 7, -9, 2, -4, 6, -8, 10} You have to modify <strong><em>HW1_p1.s</em></strong> for your implementation. Snapshot the console window and saved it as <strong><em>HW1_p1.jpg</em></strong>. Both HW1_p1.s and HW1_p1.jpg have to be submitted.




Part II: Denoising salt-and-pepper noise using the median filter.

In the previous part, you have written a code that can sort a series of numbers.

Now it can be applied to an application requiring a median filter.

Salt-and-pepper noise is impulse noise caused by sharp and sudden disturbances in image signals. Since the noise makes pixels either white or black, denoising process can be done with simply a median filter. For a 3-by-3 2D array. Applying the median filter is to sort all 9 elements in the array, and then replace the center element with the median of the sorted numbers while keeping other elements unchanged. The following example shows how the median filter works.




In this part, you are asked to apply a 3-by-3 median filter on a given 128-by-128 image with salt-and pepper noise. To reduce calculation complexity, for your convenience, the median filter is only applied to the original input array, which means the previously updated pixel values do not affect the latter filtering results. Also, we do not need to deal with boundary conditions. It means that you do not need to calculate the values when the center of the filter is on or out of the boundaries. Therefore, your final result can be represented by a 126-by-126 array.               You have to modify <strong><em>HW1_p2.s </em></strong>for your denoising implementation. Here we provide you the input data and the output printing format. The input data are the pixels as arranged below.

<table width="553">

 <tbody>

  <tr>

   <td width="92">Pixel [1]</td>

   <td width="92">Pixel [2]</td>

   <td width="92">Pixel[ 3]</td>

   <td width="81"> </td>

   <td width="103">……</td>

   <td width="92">Pixel [128]</td>

  </tr>

  <tr>

   <td width="92">Pixel [129]</td>

   <td width="92">Pixel [130]</td>

   <td width="92">Pixel [131]</td>

   <td width="81"> </td>

   <td width="103">……</td>

   <td width="92">Pixel [256]</td>

  </tr>

  <tr>

   <td width="92">Pixel [257]</td>

   <td width="92"> </td>

   <td width="92"> </td>

   <td width="81">……</td>

   <td width="103"> </td>

   <td width="92"> </td>

  </tr>

 </tbody>

</table>




You have to store the console to <strong><em>ans.txt </em></strong>for our convenience to verify your correctness. You may use ans.txt with the help of any programming language (C/C++, python, Matlab etc.) you are familiar with to check the output (126*126) image. <strong><em> </em></strong>




<u>Note:</u>

<ol>

 <li>We recommend you directly use your sort function in Part I, but should be careful about the usage of registers.</li>

 <li>We also provide you two smaller array (7*7 &amp; 15*10) as inputs for you to check your correctness when writing your code.</li>

 <li>If you have trouble in Part 2, you can write a detailed <strong><em>pdf</em></strong> to get partial credit.</li>

</ol>




Related Material:

Refer to 20191001_CompArch_SPIM_Simulator.pdf on CEIBA. A.9 SPIM (P &amp; H, p. A-40).