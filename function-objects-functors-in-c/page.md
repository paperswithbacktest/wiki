---
title: Mastering Functors in C++ for Flexible and Efficient Code
description: Functors in C++ provide stateful function objects for custom algorithms
  and efficient STL operations enabling sorting and tracking. Discover more inside
---


![Image](images/1.png)

## Table of Contents

## What is a function object (functor) in C++?

A function object, often called a functor, is a special kind of object in C++ that can be used like a function. It's created from a class or struct that overloads the `operator()`, which is the function call operator. This means you can call the object as if it were a regular function, but it can also hold its own data and state, making it more powerful than a regular function.

Functors are useful because they can keep track of information between calls. For example, if you want to count how many times a function is called, you can use a functor to keep a counter inside it. This makes them very handy in algorithms and other situations where you need to pass around a piece of code that also needs to remember things.

## How do you define a simple functor in C++?

To define a simple functor in C++, you need to create a class or struct and overload the `operator()`. This operator allows the object to be called like a function. For example, you can create a functor that adds two numbers. You would define a class called `AddFunctor` with a method `operator()` that takes two parameters and returns their sum.

Here's how you might write it: You start by defining the class `AddFunctor`. Inside this class, you define the `operator()` function. This function will take two integers as parameters and return their sum. Once you've defined this class, you can create an object of `AddFunctor` and use it like a function. For instance, if you create an object called `adder`, you can call `adder(3, 4)` and it will return `7`. This way, the functor behaves just like a regular function but can also have its own data and state if needed.

## What is the difference between a function and a functor?

A function is a piece of code that does a specific job. You call it by its name and give it some information, and it does its job and gives you back a result. For example, if you have a function called `add` that adds two numbers, you would call it like `add(3, 4)` and it would give you back `7`. Functions are simple and straightforward, but they can't remember anything between calls.

A functor, or function object, is different because it's an object that acts like a function. You make a functor by creating a class or struct and telling it how to act when it's called like a function. This is done by overloading the `operator()`, which lets you use the functor just like a function. But, unlike a regular function, a functor can also keep track of information between calls. For example, you could make a functor that counts how many times it's been called. This makes functors more powerful and flexible than regular functions.

## How can functors be used with the Standard Template Library (STL)?

Functors are really useful when you use them with the Standard Template Library (STL) in C++. The STL has a lot of algorithms and containers that can work with functors. For example, if you want to sort a list of numbers, you can use a functor to tell the `sort` function how to compare the numbers. This is great because you can make the functor do exactly what you need, like sorting numbers from highest to lowest instead of the usual lowest to highest.

Another way functors help with the STL is by keeping track of things while the algorithm runs. For instance, if you're using the `for_each` function to go through a list and do something to each item, you can use a functor to count how many times it's been called or to remember some information about the items it's seen. This makes your code more powerful and easier to understand because the functor can do its job and keep track of things at the same time.

## What are the benefits of using functors over regular functions?

Functors are better than regular functions because they can remember things between calls. Imagine you have a function that counts how many times it's been called. With a regular function, you'd need to keep the count somewhere else, but a functor can keep the count inside itself. This makes your code simpler and easier to understand because the functor can do its job and keep track of things at the same time.

Another benefit of functors is that they can be used with the Standard Template Library (STL) in C++. The STL has lots of tools that work well with functors. For example, if you want to sort a list of numbers, you can use a functor to tell the sorting tool how to compare the numbers. This lets you do things like sorting from highest to lowest, which is harder to do with regular functions. Functors make your code more powerful and flexible because they can be used in many different ways with the STL.

## How do you implement a functor with state?

To implement a functor with state, you create a class or struct that has some data inside it. This data is the state that the functor can remember between calls. For example, you can make a functor that counts how many times it's been called. You would put a counter inside the functor and every time the functor is called, it adds one to the counter. This way, the functor can keep track of how many times it's been used, even if you call it from different parts of your program.

When you want to use this functor, you define the `operator()` function inside the class. This function does whatever job you want the functor to do, and it can also update the state. For instance, if you're counting calls, the `operator()` function would add one to the counter each time it's called. After you've set up the class with the state and the `operator()` function, you can create an object of this class and use it just like a regular function. But because it's a functor, it will remember the state, like the number of times it's been called, even between different uses.

## What is the role of the `operator()` in functors?

The `operator()` is a special function in C++ that makes a class or struct act like a function. When you put this function inside a class, you create what's called a functor, or function object. This means you can call the object just like you would call a regular function, but it can also keep track of information between calls. For example, if you want to count how many times something happens, you can put a counter inside the functor and have the `operator()` add one to the counter each time it's called.

The `operator()` is important because it lets the functor do its job and remember things at the same time. This makes functors more powerful than regular functions. For instance, if you're sorting a list of numbers, you can use a functor to tell the sorting tool how to compare the numbers. The `operator()` would be the part that does the comparing, and it can also keep track of other information if you need it to. This makes your code more flexible and easier to use with tools like the Standard Template Library (STL).

## How can you use lambda expressions as functors?

Lambda expressions are a short way to make small, one-time-use functions in C++. They can act like functors because they can keep track of information between calls. You make a lambda expression by using the `[capture]` part to grab any information you want it to remember, then the `(parameters)` part to say what information it needs when you call it, and the `{body}` part to tell it what to do. For example, if you want to count how many times a function is called, you can use a lambda expression to keep a counter inside it. You would write something like `[count = 0]() mutable { return ++count; }` to make a lambda that counts up each time you call it.

When you use lambda expressions as functors, they're handy because they can be used right where you need them, without having to make a whole class. For instance, if you're sorting a list of numbers and want to sort them from highest to lowest, you can use a lambda expression to tell the sorting tool how to compare the numbers. You might write something like `[](int a, int b) { return a > b; }` to make a lambda that sorts the numbers from highest to lowest. This makes your code simpler and easier to understand because the lambda can do its job and keep track of things at the same time, just like a functor.

## What are higher-order functors and how are they implemented?

Higher-order functors are like regular functors but with an extra twist. They are functors that can take other functors as arguments or return functors as results. This makes them very powerful because they can work with other pieces of code that act like functions. For example, you might have a higher-order functor that takes a functor that adds numbers and another that multiplies numbers, and then it uses both to do some fancy math.

To implement a higher-order functor, you start by making a class or struct that has a `operator()` function. Inside this function, you can take another functor as a parameter and use it to do something. For instance, if you want to make a higher-order functor that applies two different functors to a number, you would define the `operator()` to take two functors and a number, and then it would use the functors to change the number in some way. This way, the higher-order functor can work with other functors to do more complex jobs.

## How do you use functors for custom sorting in C++?

Functors are really helpful when you want to sort things in a special way in C++. Imagine you have a list of numbers and you want to sort them from highest to lowest instead of the usual lowest to highest. You can make a functor that tells the sorting tool how to compare the numbers. For example, you could create a class called `SortDescending` with an `operator()` function that takes two numbers and returns `true` if the first number is bigger than the second. Then, when you use the `sort` function from the Standard Template Library (STL), you can pass your `SortDescending` functor to it, and it will sort the numbers from highest to lowest.

Using functors for custom sorting is great because they can do more than just compare numbers. They can also keep track of information while sorting. For instance, if you want to sort a list of people by their age but also count how many people are over a certain age, you can make a functor that does both. The functor would have an `operator()` function that compares ages and a counter inside it that goes up every time it sees someone over the age you're interested in. This way, after sorting, you not only have the list sorted by age, but you also know how many people are over a certain age, all thanks to the functor.

## What are the performance implications of using functors?

Using functors can make your code run faster because they can be inlined by the compiler. When the compiler inlines a function, it puts the code of the function right where it's called instead of jumping to another place in the code. This can save time because the computer doesn't have to do as much work to call the function. Functors are more likely to be inlined than regular functions because they are objects and the compiler can see their whole definition, which makes it easier to optimize.

On the other hand, functors can also use more memory because they are objects. Every time you make a functor, it takes up space in memory, and if you make a lot of them, this can add up. But usually, the benefits of using functors, like being able to keep track of information and being faster because of inlining, outweigh the extra memory they use. So, functors can be a good choice if you need to do some fancy things with your code and want it to run quickly.

## How can you combine functors to create more complex operations?

Combining functors can help you do more complicated things in your code. Imagine you have two functors, one that adds numbers and another that multiplies them. You can make a new functor that uses both of these to do something more fancy, like adding two numbers and then multiplying the result by another number. To do this, you make a new class with an `operator()` function that takes the two original functors as parameters. When you call this new functor, it uses the other functors to do its job, making your code more powerful and flexible.

This way of combining functors is useful when you want to break down a big job into smaller parts. For example, if you're sorting a list of people by their age and then by their name, you can make one functor that compares ages and another that compares names. Then, you can make a third functor that uses both of these to sort the list first by age and then by name. This makes your code easier to understand and change because you can work on each part separately and then put them together to do the whole job.

## References & Further Reading

[1]: Meyers, S. (2014). ["Effective Modern C++: 42 Specific Ways to Improve Your Use of C++11 and C++14"](https://www.amazon.com/Effective-Modern-Specific-Ways-Improve/dp/1491903996). O'Reilly Media.

[2]: Jansen, S. (2020). ["Machine Learning for Algorithmic Trading: Predictive models to extract signals from market and alternative data for systematic trading strategies with Python"](https://www.amazon.com/Machine-Learning-Algorithmic-Trading-alternative/dp/1839217715). Packt Publishing.

[3]: Chan, E. P. (2008). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://github.com/ftvision/quant_trading_echan_book). John Wiley & Sons.

[4]: LeVeque, R. J., Mitchell, I. M., & Strohmer, T. (Editors) (2020). ["Financial Mathematics, Derivatives, and Simulation"](https://tevza.org/home/course/modelling-II_2016/books/Leveque%20-%20Numerical%20Methods%20for%20Conservation%20Laws.pdf). Springer.

[5]: Lopez de Prado, M. (2018). ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089). Wiley.