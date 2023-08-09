# STL Data Structure

[toc]

## Vector

- Header file
        
        include<vector>

- Define the `std::vector`

        template<class Type, class Allocator = std::allocator<Type>> class vector;

    - `Type` – is the type of element contained in the `std::vector`. It can be any valid C++ type or even a user-defined type.

    - `Allocator` - is used to acquire/release memory and to construct/destroy the elements in that memory.

- Functions associated with `std::vector`
    - `begin()` – Returns an iterator pointing to the first element in the vector
    - `end()` – Returns an iterator pointing to the theoretical element that follows the last element in the vector
    - `size()` – Returns the number of elements in the vector.
    - `front()` – Returns a reference to the first element in the vector
    - `back()` – Returns a reference to the last element in the vector
    - `assign()` – Assigns new value to the vector elements by replacing old ones
    - `push_back()` – Push the elements into a vector from the back
    - `pop_back()` – Pop or remove elements from a vector from the back.
    - `insert()` – Inserts new elements before the element at the specified position
    - `erase()` – Remove elements from a container from the specified position or range.
    - `clear()` – Remove all the elements of the vector container

## Set

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

## Map

- Header File

        include <map>

- Define the `std::list`

        template<class Key, class Type, class Compare = std::less<Key>, class Allocator = std::allocator<std::pair<const Key, T>>> class map;

    - `Key` - is the type of the keys. Each element in a map is uniquely identified by its key value. It can be any valid C++ type or even a user-defined type.
    - `Type` – is the type of the mapped value. Each element in a map stores some data as its mapped value. It can be any valid C++ type or even a user-defined type.
    - `Compare` - is a binary predicate that takes two element keys as arguments and returns a bool. The expression `comp(a,b)`, where `comp` is an object of this type and `a` and `b` are key values, shall return true if `a` is considered to go before `b` in the strict weak ordering the function defines.
    - `Allocator` - is used to acquire/release memory and to construct/destroy the elements in that memory.

- Functions associated with `std::map`

    - `operator[]` - Access element
    - `begin()` – Returns an iterator to the first element in the map.
    - `end()` – Returns an iterator to the theoretical element that follows the last element in the map.
    - `size()` – Returns the number of elements in the map.
    - `empty()` – Returns whether the map is empty.
    - `insert({keyvalue, mapvalue})` – Adds a new element to the map.
    - `erase(iterator position)` – Removes the element at the position pointed by the iterator.
    - `erase(const g)` – Removes the key-value ‘g’ from the map.
    - `clear()` – Removes all the elements from the map.