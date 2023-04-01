# Activities

## Task 1

- What are the advantages of the C++ Standard Template Library (STL):
# V:
Reusability: STL provides a set of standard data structures and algorithms that can be reused across multiple projects, reducing development time and effort.

Efficiency: STL is designed to be efficient, with algorithms and data structures that are optimized for performance.

Portability: STL is a part of the C++ standard, so it is available on all platforms that support C++. This ensures that code written using STL is portable across different operating systems and hardware.

Consistency: STL provides a consistent set of interfaces for different data structures and algorithms, making it easy to learn and use.

Safety: STL provides type-safe and memory-safe data structures and algorithms, helping to prevent errors and bugs in code.

- What are the disadvantages of STL?
# V:
Complexity: STL can be complex to learn and use, especially for beginners, due to its large number of data structures and algorithms.

Compilation time: STL code can take longer to compile than handwritten code, especially for large programs.

Debugging: Debugging STL code can be difficult due to the use of templates, which can make the code harder to read and understand.

- What are the main components of STL?
# V:
Containers: Containers are data structures that store a collection of elements, such as vectors, lists, maps, and sets.

Iterators: Iterators are objects that allow you to traverse the elements of a container.

Algorithms: Algorithms are functions that operate on containers, such as sorting, searching, and merging.

Function Objects: Function objects are objects that behave like functions, and can be used with algorithms that take functions as arguments.

Adapters: Adapters are classes that modify the behavior of existing containers or algorithms, such as stack, queue, and priority_queue.

> You can refer to the following link: https://www.geeksforgeeks.org/the-c-standard-template-library-stl/

## Task 2

- Refer to `./src/non-manipulative.cpp`
  - Discuss how the program works
  Program demonstrates the working of some of the functions provided by the C++ Standard Template Library (STL) for working with vectors

  The program first prints the initial vector, then sorts it in ascending order and prints it again, then sorts it in descending order and prints it again, then reverses it and prints it again. Finally, it finds the maximum and minimum elements of the vector, and calculates the sum of all its elements.

  What are the Non-Manipulating Algorithms used in the program?

  Max_ & Min_element(), Accumulate() These functions are called non-manipulating algorithms because they do not modify the contents of the vector. Instead, they operate on the elements of the vector and return some information about them.

  - What are the Non-Manipulating Algorithms used in the program?
  # V:
  Max_ & Min_element(), Accumulate() These functions are called non-manipulating algorithms because they do not modify the contents of the vector. Instead, they operate on the elements of the vector and return some information about them.

- Refer to `./src/manipulative.cpp`
  - Discuss how the program works
  # V:
  Program demonstrates the usage of the erase() function in the C++ STL library to remove elements from a vector.

  The program first initializes a vector vect with an array of integers. It then displays the contents of the vector using a for loop. It then removes the element with the value 10 from the vector and displays the modified vector. Finally, it removes all the duplicate elements from the vector and displays the final vector.

  - What are the Manipulating Algorithms used in the program?
  # V:
  None are used in the example.

> You can refer to the following link: https://www.geeksforgeeks.org/c-magicians-stl-algorithms/

## Task 3

- Refer to the following article. Reflect on the difference between Big Oh and little oh
  https://www.baeldung.com/cs/big-o-vs-little-o-notation
  # V:
  Big O and little o notations are both used to analyze the performance of algorithms, but Big O is used to estimate the worst-case scenario, while little o is used to estimate the best-case scenario.

## Task 4

Refer to one of the following articles. Reflect on the differences between Big Oh, Big Omega and Theta.
# V:
Big O notation is used to describe the upper bound of the growth rate of an algorithm's time or space complexity. In other words, it gives an estimate of the worst-case scenario for an algorithm. For example, if an algorithm has a time complexity of O(n^2), it means that the time taken by the algorithm to complete its execution will increase proportionally with the square of the input size.

Big Omega notation is used to describe the lower bound of an algorithm's growth rate. It gives an estimate of the best-case scenario for an algorithm. If an algorithm has a time complexity of Ω(n^2), it means that the time taken by the algorithm to complete its execution will increase at a rate that is at least the square of the input size.

Theta notation, on the other hand, is used to describe both the upper and lower bounds of an algorithm's growth rate. If an algorithm has a time complexity of Θ(n^2), it means that the time taken by the algorithm to complete its execution will increase proportionally with the square of the input size, but no faster or slower than that.

In summary, Big O represents the upper bound of the growth rate of an algorithm's time or space complexity, Big Omega represents the lower bound of an algorithm's growth rate, while Theta represents both the upper and lower bounds of an algorithm's growth rate.

- https://jarednielsen.com/big-o-omega-theta/
- https://www.codeandgadgets.com/big-oh-big-omega-and-theta-definitions/
- https://www.geeksforgeeks.org/difference-between-big-oh-big-omega-and-big-theta/
