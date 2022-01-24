# DEV-09: The Libuv Thread Pool

## Tags: []

## Links: <https://www.udemy.com/course/advanced-node-for-developers/learn/lecture/9636112#overview>

## What are these Libraries demonstrating threading like behavior?

    The Libuv module has another responsibility that is relevant for some very particular functions in the standard node.js library. 

    For SOME of the standard library function calls, the Node C++ and Libuv 
    decide to do expensive calculations outside of the event loop entirely.
    Instead they make use of something called the tread pool.


## What is the thread pool?

    The thread pool is a series of four threads that can be used for running computationally intensive tasks such as the crypto library's PBKDF2 function

## What does this all mean?

    SO that means that in addition to the thread used for the event loop, there are 4 other threads that can be used to offload expensive calculations that need to occur inside of our application.

    Many of the functions, including the node standard library, will automatically make use of theis thread pool.


## So is Node.js truly single threaded?

    The Event loop is single threaded
    The Libuv thread pool is not, and has by default 4 threads
    Together they make up node.js and so it a mix of both






