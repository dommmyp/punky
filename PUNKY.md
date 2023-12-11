 
Part 1: Comprehension Questions

Suppose statement2 may throw an exception in the following two codes: 
// Code A                                // Code B
try{                                     try{
    statement1;                              statement1;
    statement2;                              statement2;
    statement3;                              statement3;
}                                         }
catch(Exception ex1){                     catch(Exception ex1){
    System.exit(0);                           return;
}                                         }
finally{                                  finally{
   statement4;                                statement4;
}                                         }
statement5;                               statement5;

 
Answer the following questions:
If no exception occurs, will statement3, statement4 or statement5 be executed?
If an exception of type Exception is thrown, will statement3, statement4 or statement5 be executed?
If an exception that is not of type Exception is thrown, will statement3, statement4 or statement5 be executed?


Evaluate the following postfix expression using a stack. Show all the steps.
20 6 * 6 5 * 31 + 1 - / 9 *

Determine the exact number of iterations executed by the following code and the time complexity of the code using Big-O notation? Show your work.



for (int i = n; i > 0; --i)
 for (int j = n/20; j > 0; j /= 2)  
  for(int k = 1; k < n; k *= 3)    	 
    product = i * k + j * (k-2) + k;
 

Assume the following list of values {18, 9, 32, 22, 75, 83, 3} to be sorted using mergesort. Show all the steps to sort the list.
 
Assume the following list of values {16, 80, 22, 55, 64, 95, 25} to be sorted using quicksort. Use a pivot as the first element of the list. Show the steps to sort the list.
 
The nodes in a binary tree in pre-order and in-order sequences are as follows:
Pre-order: A B C D E F G H I
In-order: D C B A F E G I H
Draw the binary tree and write the post-order traversal of the tree.
 
Remove the node with value 9 from the following binary search tree. Write the in-order traversal of the BST after the deletion.

Redraw the following max heap after adding a node with value 92 and rebuilding the heap. Write the list of the nodes as stored in the heap’s array list.

Assume a hash table has the initial size 4 and its load factor is 0.5, show the hash table after inserting the keys 34, 29, 53, 44, 120, 39, and 45, using linear probing.

  Assume a hash table has the initial size 4 and its load factor is 0.9, show the hash table after inserting the keys 34, 29, 53, 44, 120, 39, and 45, using separate chaining.

Part 2: Programming Questions

Write a recursive method to compute the following series:
 		M(n) = 1 + 13+ 25+ . . . +n2n+1

Write a test program that displays M(n) for n = 1, 2, . . ., 10
 
Write a recursive method that returns the reverse of a string s.

 Write a generic recursive method removeDuplicates that removes duplicates from an ArrayList. The method returns a new ArrayList that contains the distinct elements from the original list.

Write a generic method max that finds the maximum value in an ArrayList.

Add the methods addAll(ArrayList<E>), removeAll(ArrayList<E>), retainAll(<ArrayList<E>), and toArray() to the classes ArrayList and determine their time complexity.
 
[1, 2, 3].addAll([3, 4]) results in the first list equal to [1, 2, 3, 3, 4]
[1, 2, 3].removeAll([3, 4]) results in the first list equal to [1, 2]
[1, 2, 3].retainAll([3, 4]) results in the first list equal to [3]
[1, 2, 3].toArray() returns the array {1, 2, 3}
 
Add the methods get(int index), set(int index, E value), lastIndexOf(E value) to the class  LinkedList  (singly linked list) and determine their time complexity.

Add a method reverse() to the class LinkedList (singly linked list) to print the elements of the list in reverse order (from the last element to the first element). Determine the time complexity of the method.

Write a test program that stores 5 million integers in a singly linked list and test the time to traverse the list using an iterator vs. using the method get(index).

 The quicksort algorithm covered in class selects the first element in the list as the pivot. Revise it by selecting the median among the first, middle, and the last elements in the list. Compare the two quicksort algorithms on three arrays. The first array contains random integers, the second is sorted and the third is in reverse order.

 Implement the clone and equals methods for the BST class. Two BST trees are equal if they contain the same nodes. The clone method returns a deep copy of the tree. Determine the time complexity of the two methods.

 Add the following methods to the BST class.
// Iterative preorder traversal using a stack
// No recursion
public void iterativePreorder()

// Recursive search method
public boolean recursiveSearch(E item)

 
The class HashMap seen in class uses a LinkedList to store collisions. Replace LinkedList with BST. The generic type K must be  Comparable. Redefine HashMap and test it using the same test program from ALA 10.

 Add the following methods to the class HashMap:
public ArrayList<K> keys(): returns an array list with all the keys in the hash table.
public boolean containsValue(V val): returns true if the hashmap has one or more keys mapped to the specified value val.

 Implement the hierarchy of classes shown below. Write a program that reads the files patients.txt, doctors.txt, and billings.txt, and prints out the total income from the Billing records, the highest total income of doctors, and the highest total spending of patients. Note that Person is an abstract class.


  Suppose you have a collection of student records in the file students.txt. The records contain the name and grade of a student. The records are maintained in an array list. Write a program that fetches data from the text file and builds the array list of student records, then sorts the list by name, calculates the maximum and minimum grades, and the class average. Write a method that separates the students in the list into two lists, one containing records of passing students and one containing records of failing students (use a grade of 60 or more for passing). You are asked to do this in two ways:
Create a second list of passing students and a third list of failing students
Create a second list of failing students and copy the records of failing students to the new list and remove them from the original list.
Repeat the two solutions in a and b using a singly linked list.
Analyze the time and space complexity of the two solutions for each data structure and compare them.
