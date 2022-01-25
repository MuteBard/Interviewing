# Talking

## What is Node js?

    Node.js is a collection of dependecies and APIs's that ultimately allow us to write javascript outside of the browser and on our machines. The dependencies also allow us to work with OS operations such as Networking, Concurrancy and File systems.

## What is the Event Loop?

    The Event loop is like a control structure that decides what our single thread should be doing at any given point in time. Each iteration or tick of the Event loop is dictated by a series of conditions that it determines from the code that we write.

    Whether there are any pending setTimeout, setInterval or setImmediate
    Whether there are any pending Operating System Task like an http request
    Whether there are pending long running operations such as checking the file system

    If the event loop performs a tick and any of these turn out to be the case then the loop occurs for another tick. It also waits for any potential future events and closes any streams. Alot of performance concerns in node are tied to how the event loop behaves.

## Explain callback in Node.js.

    A callback function is called after a given task. It allows other code to be run in the meantime and prevents any blocking.

## What are the advantages of using promises instead of callbacks?

    - The control flow of asynchronous logic is more specified and structured.
    - The coupling is low.
    - We've built-in error handling.
    - Improved readability.
