# DEV-10: Outside notes

## Why is Node.js Single-threaded?

    Node.js is single-threaded for async processing. By doing async processing on a single-thread under typical web loads, more performance and scalability can be achieved instead of the typical thread-based implementation.

## If Node.js is single-threaded, then how does it handle concurrency?

    The Multi-Threaded Request/Response Stateless Model is not followed by the Node JS Platform, and it adheres to the Single-Threaded Event Loop Model. The Node JS Processing paradigm is heavily influenced by the JavaScript Event-based model and the JavaScript callback system. As a result, Node.js can easily manage more concurrent client requests. The event loop is the processing model's beating heart in Node.js.

## Explain callback in Node.js.

    A callback function is called after a given task. It allows other code to be run in the meantime and prevents any blocking.  Being an asynchronous platform, Node.js heavily relies on callback. All APIs of Node are written to support callbacks.

## What are the advantages of using promises instead of callbacks?

    - The control flow of asynchronous logic is more specified and structured.
    - The coupling is low.
    - We've built-in error handling.
    - Improved readability.
