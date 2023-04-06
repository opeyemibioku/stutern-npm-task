### What is the Event loop ?

#### The event loop is a fundamental concept in the Node.js runtime environment responsible for executing the code, collecting and processing events, and executing queued sub-tasks making it well-suited for building scalable and high-performance applications.

### Explain the 6 phases of the event loop

#### Timers: This phase executes all the callbacks scheduled by setTimeout() and setInterval(). The callbacks are executed in the order they were scheduled, and the amount of time that has elapsed since the timer was set is taken into account.

#### I/O callbacks: This phase executes all the I/O-related callbacks, such as those associated with reading from a file or making a network request. These callbacks are called when their corresponding I/O operations have completed.

#### Preparation/idle phase: These phases are used internally by Node.js and are generally not of interest to most developers.

#### I/O polling: In this phase, Node.js waits for new I/O events to occur, such as incoming network requests or completed database queries. If there are no events to process, Node.js will block and wait for new events to arrive.

#### setImmediate() callbacks execution: This phase executes all the callbacks that were scheduled by setImmediate(). These callbacks are executed immediately after the current poll phase completes.

#### Close events callbacks.: This phase executes all the callbacks that were registered to be called when a resource is closed, such as a database connection or a server socket.

### List some best practices in server-side code development

#### Use a version control system such as Git

#### Use error handling

#### Document your code

#### Break your code into small, reusable modules

#### Keep dependencies up-to-date

### What is NPM5: How do you initialize a package in npm

#### A package is initialized using npm init

### How do you run a script in the package.json ?

#### To run a script that in the package.json file, you use the "npm run" command followed by the script name.
