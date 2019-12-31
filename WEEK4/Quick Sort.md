## Quick Sort

Quick Sort(快速排序法)是一種「把大問題分成小問題處理」的Divide and Conquer方法，

數列中任意挑選一個數，稱為pivot，然後調整數列，使得「所有在pivot左邊的數，都比pivot還小」，而「在pivot右邊的數都比pivot大」。

接著，將所有在pivot左邊的數視為「新的數列」，所有在pivot右邊的數視為「另一個新的數列」，

「分別」重複上述步驟(選pivot、調整數列)，直到分不出「新的數列」為止。

! [image] C:\Users\Administrator\Desktop\Quicksort流程圖.png