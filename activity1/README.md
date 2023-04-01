# Activities

---

> [Course Feedback](https://ojp.metropolia.fi/lomakkeet/1/lomake.html?code=VFQwMEZFMzktMzAwMQ==)

---

## Task 1

- What is the difference between function overloading and function templates. You can refer to the programs in the `./src/` folder as well as [Links 2 and 3](#links) below.

# Vastaus:
Function overloading is a technique in which multiple functions with the same name are defined in a program, but they differ in the type and/or number of arguments they take. When a function call is made with a particular set of arguments, the compiler selects the appropriate function based on the type and number of arguments provided. This allows for more flexibility in function calls and can help reduce code duplication.

Function templates, on the other hand, are a way of defining generic functions that can be used with different data types. A function template is a blueprint for a function that takes one or more type parameters as inputs, which are used to specify the types of the arguments and return value. When a function call is made with a particular set of arguments, the compiler generates a new function by substituting the template parameters with the actual types provided in the function call.

In summary, function overloading provides different implementations of a function based on the type and number of arguments, while function templates provide a generic implementation of a function that can be used with different data types.

- Rewrite the following program using templates

```cpp
#include <iostream>

int add(int x, int y)
{
    return x + y;
}

double add(double x, double y)
{
    return x + y;
}

int main()
{
    std::cout << add(1, 2); // calls add(int, int)
    std::cout << '\n';
    std::cout << add(1.2, 3.4); // calls add(double, double)

    return 0;
}
```
# Vastaus:
#include <iostream>

template <typename T>
T add(T x, T y)
{
    return x + y;
}

int main()
{
    std::cout << add(1, 2); // calls add<int>(int, int)
    std::cout << '\n';
    std::cout << add(1.2, 3.4); // calls add<double>(double, double)

    return 0;
}

## Task 2

Refer to the following link:
https://www.softwaretestinghelp.com/vectors-in-stl/

Discuss the difference between

- Size() and capacity()
 # V:
 size() returns the number of elements currently stored in the vector, while capacity() returns the maximum number of elements that the vector can store without allocating more memory. The size() of a vector can change as elements are added or removed, but the capacity() only changes when the vector needs to allocate more memory to accommodate additional elements.

- begin() and cbegin()
# V:
begin() returns an iterator to the first element in the vector, while cbegin() returns a constant iterator to the first element. This means that the cbegin() iterator cannot be used to modify the contents of the vector. Both begin() and cbegin() are used to traverse the vector from the beginning to the end.

- end() and cend()
# V:
end() returns an iterator to the element following the last element in the vector, while cend() returns a constant iterator to the element following the last element. This means that the cend() iterator cannot be used to modify the contents of the vector. Both end() and cend() are used to traverse the vector from the beginning to the end.

In summary, size() and capacity() are used to determine the number of elements in the vector and the amount of memory allocated for the vector, respectively. begin() and cbegin() are used to obtain an iterator to the first element in the vector, while end() and cend() are used to obtain an iterator to the element following the last element in the vector. The difference between begin() and cbegin(), and end() and cend() is that the latter set returns a constant iterator, which cannot be used to modify the contents of the vector.

## Links

1. https://cpp.sh/
2. https://www.learncpp.com/cpp-tutorial/function-templates/
3. https://www.learncpp.com/cpp-tutorial/function-overload-differentiation/
4. https://www.geeksforgeeks.org/design-and-analysis-of-algorithms/
