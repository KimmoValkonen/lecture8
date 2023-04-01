# Activities

## Task 1

> Refer to the following links while discussing the answer.

- What is the difference between `array` and `std::array`
  https://stackoverflow.com/questions/30263303/stdarray-vs-array-performance
  # Vastaus:
  Type safety: std::array is a type-safe container that prevents the user from accessing elements outside of the array bounds at compile-time. In contrast, array does not have this safety feature, and out-of-bounds access can lead to undefined behavior at runtime.

  Size: The size of an array must be known at compile-time, while the size of an std::array can be specified at runtime, but is fixed for the lifetime of the container.

  Functions and algorithms: std::array provides member functions and algorithms that make it easier to work with the container, such as at(), front(), back(), fill(), swap(), and sort(). These functions and algorithms are not available for array.

  Compatibility: std::array is compatible with the algorithms provided by the C++ Standard Library, such as std::for_each(), std::transform(), and std::accumulate(). array is not directly compatible with these algorithms, as it does not provide the required member functions.

  Regarding performance, std::array is generally as fast as built-in arrays because it provides the same memory layout and efficient element access. In fact, std::array may be faster in some cases because it is type-safe and allows for range checking at compile-time, which can lead to faster code. However, in cases where performance is critical, it is best to benchmark the two options to determine the best choice for a specific use case
- What is the difference between `std::array` and `std::vector`
  https://www.softwaretestinghelp.com/arrays-in-stl/
  # V:
  Size: std::array has a fixed size that is specified at compile-time, while std::vector can dynamically grow or shrink at runtime.

  Memory allocation: std::array allocates its elements on the stack, while std::vector dynamically allocates its elements on the heap.

  Accessing elements: std::array provides constant-time access to its elements through the use of the [] operator, while std::vector provides constant-time access to its elements through the use of the [] operator and iterators.

  Range checking: std::array does not perform any range checking when accessing its elements, while std::vector provides range checking for its elements through the use of the at() function.

  Performance: std::array is generally faster than std::vector for small, fixed-size containers because it does not require dynamic memory allocation. However, for large or dynamically changing containers, std::vector may be faster because it can allocate memory dynamically and avoid the cost of copying elements when resizing.

  Compatibility: std::array is compatible with C-style arrays and can be used in functions that expect a C-style array argument, while std::vector cannot be used in this way.

  In summary, std::array is a fixed-size container that provides fast and efficient access to its elements, while std::vector is a dynamic container that can grow or shrink at runtime and provides more flexible memory management. The choice between the two depends on the specific use case and the requirements for performance, memory management, and size flexibility.

- What is the difference between `std::list` and `std::vector`
  https://www.softwaretestinghelp.com/lists-in-stl/

  # V:
  Memory allocation: std::vector uses contiguous memory to store its elements, while std::list uses a linked list structure. This means that inserting or erasing elements in the middle of a std::vector can be expensive due to the need to move elements to make room or fill gaps. In contrast, inserting or erasing elements in the middle of a std::list is generally fast because it only requires changing pointers to link the neighboring nodes.

  Accessing elements: std::vector provides fast constant-time access to its elements through the use of the [] operator and iterators, while std::list does not support random access and requires iterating through the list to access elements. This means that accessing elements in a std::list can be slower than in a std::vector because of the need to traverse the linked list.

  Iterators: std::vector provides both forward and reverse iterators, while std::list provides bidirectional iterators that can traverse the list in both directions.

  Insertion and erasure: std::vector provides efficient insertion and erasure of elements at the end of the container, but less efficient for elements in the middle. std::list provides efficient insertion and erasure of elements at any position due to its linked list structure.

  Size: std::vector can dynamically grow or shrink at runtime, while std::list can dynamically grow at runtime but not shrink because of its linked list structure.

  Memory overhead: std::vector has a lower memory overhead than std::list due to its contiguous memory allocation. std::list requires extra memory for the pointers that link the nodes of the linked list.

  In summary, std::vector is a container that provides efficient random access to its elements and fast insertion and erasure at the end of the container. std::list is a container that provides efficient insertion and erasure of elements at any position and bidirectional iteration, but slower access to its elements. The choice between the two depends on the specific use case and the requirements for memory management, access patterns, and insertion and erasure performance.

## Task 2

- Run the Stack and Queue examples in the following link
  https://www.softwaretestinghelp.com/stacks-and-queues-in-stl/

> make sure you correct the syntax e.g `&lt;int&gt; becomes  <int>`
# V:
Tehtiin harjoitus ajamalla cpp:ssä

## Task 3

- Discuss the different types of iterators present in C++. You can refer to the following link
  https://www.geeksforgeeks.org/introduction-iterators-c/
- What are the Benefits of Iterators
# V:
Iterator is an object that points to an element in a container such as an array, vector, list, map, etc. Iterators allow you to access the elements of a container in a sequential manner, without knowing the underlying implementation of the container. Here are the different types of iterators in C++:

Input Iterator: It is used to read values from a container, but not modify them. It supports increment, dereference and comparison operators.

Output Iterator: It is used to write values to a container, but not read them. It supports increment and dereference operators.

Forward Iterator: It is similar to the Input Iterator, but it can be used to modify the values of a container. It supports all the operations of Input Iterator, as well as increment, dereference and assignment operators.

Bidirectional Iterator: It is similar to Forward Iterator, but it supports backward movement as well. It supports all the operations of Forward Iterator, as well as decrement operator.

Random Access Iterator: It is the most powerful iterator, as it supports all the operations of Bidirectional Iterator, as well as arithmetic operations like addition and subtraction.

Benefits of iterators:

Abstraction: Iterators provide a layer of abstraction between the container and the code that uses it. This allows you to write generic algorithms that work with any container, without having to know the details of its implementation.

Efficiency: Iterators are designed to be efficient, and can be used to access the elements of a container in constant time.

Flexibility: Iterators can be used to traverse a container in any order, and can be used to modify the elements of a container as well.

Safety: Iterators provide a safe way to access the elements of a container, as they prevent you from accessing elements that are out of bounds. They also provide a safe way to modify the elements of a container, as they prevent you from modifying elements that are read-only.

## Links

- https://cpp.sh/
