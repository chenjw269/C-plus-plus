# STL Data Structure

[toc]

## Stack

- Header file
        
        include<stack>

- Define the `std::stack`

        template <class Type, class Container = std::deque<Type>> class stack;

    - `Type` – is the type of element contained in the `std::stack`. It can be any valid C++ type or even a user-defined type.

    - `Container` – is the type of underlying container object.

- Functions associated with `std::stack`
    - `empty()` – Returns whether the stack is empty
    - `size()` – Returns the size of the stack
    - `top()` – Returns a reference to the top most element of the stack
    - `push(g)` – Adds the element ‘g’ at the top of the stack
    - `pop()` – Deletes the most recent entered element of the stack

## List

- Header File

        include <list>

- Define the `std::list`

        template<class Type, class Allocator = std::allocator<Type>> class list;

    - `Type` – is the type of element contained in the `std::list`. It can be any valid C++ type or even a user-defined type.

    - `Allocator` - is used to acquire/release memory and to construct/destroy the elements in that memory.

- Functions associated with `std::list`
    - `front()` – Returns the value of the first element in the list.
    - `back()` – Returns the value of the last element in the list.
    - `push_front()` – Adds a new element ‘g’ at the beginning of the list.
    - `push_back()` – Adds a new element ‘g’ at the end of the list.
    - `pop_front()` – Removes the first element of the list, and reduces the size of the list by 1.
    - `pop_back()` – Removes the last element of the list, and reduces the size of the list by 1.
    - `insert()` – Inserts new elements in the list before the element at a specified position.
    - `size()` – Returns the number of elements in the list.
    - `begin()` – Returns an iterator pointing to the first element of the list.
    - `end()` – Returns an iterator pointing to the theoretical last element which follows the last element.

## Deque