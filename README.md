# NodeJS Questions

Some common node.js questions and answers.

###### 1. Which one is the node global object?

- A: log
- B: import
- C: process
- D: http

<details><summary><b>Answer</b></summary>

#### Answer: C

`process` is one of the node global object. Global objects are globally accessible. These are, <b>**dirname</b>, <b>**filename</b>, <b>module</b>, <b>process</b>, <b>setTimeout</b>, <b>setInterval</b>, <b>setImmediate</b>.

</details>

###### 2. Which module is used to provide compression and decompression functionalities?

- A: net
- B: buffer
- C: zlib
- D: dns

<details><summary><b>Answer</b></summary>

#### Answer: C

`zlib` module provides compression(zip) and decompression(unzip) functionalities.

</details>

###### 3. Which console method is used to show the stack trace?

- A: stack
- B: log
- C: trace
- D: debug

<details><summary><b>Answer</b></summary>

#### Answer: C

`trace` method is used to show the stack trace.

</details>

###### 4. Which module would you use to get the server information?

- A: dns
- B: url
- C: net
- D: tls

<details><summary><b>Answer</b></summary>

#### Answer: A

`dns` module is used to get the server information.

</details>

###### 5. Which one is used to read a file asynchronously?

- A: fs.getFile
- B: fs.read
- C: fs.readFile
- D: fs.get

<details><summary><b>Answer</b></summary>

#### Answer: C

`fs.readFile` is used to read a file asynchronously.

</details>

###### 6. Which module would you use to encrypt data?

- A: crypto
- B: process
- C: encrypt

<details><summary><b>Answer</b></summary>

#### Answer: A

`crypto` module is used to encrypt data.

</details>

###### 7. Which method is used to exit(kill) in node.js?

- A: kill
- B: exit
- C: stop

<details><summary><b>Answer</b></summary>

#### Answer: B

`process.exit()` is used to exit in node.js.

</details>

###### 8. Which one is the core module of node?

- A: require
- B: import
- C: fs
- D: process

<details><summary><b>Answer</b></summary>

#### Answer: C

`fs` is a core module of node. Some of them are, <b>buffer</b>, <b>crypto</b>, <b>dns</b> etc.

</details>

###### 9. Which command is used to tell node to run javascript strict mode in node repl?

- A: node -strict
- B: node --strict
- C: node --use-strict
- D: node -use--strict

<details><summary><b>Answer</b></summary>

#### Answer: C

`node --use-strict` will run node in javascript strict mode.

</details>

###### 10. Which one is not a node repl command?

- A: .save
- B: .clear
- C: .help
- D: .find

<details><summary><b>Answer</b></summary>

#### Answer: D

`.find` is not a node repl command. The repl commands are, <b>.break</b>, <b>.clear</b>, <b>.editor</b>, <b>.exit</b>, <b>.help</b>, <b>.load</b>, <b>.save</b>.

</details>

###### 11. Which one is an instance of Event Emitter?

- A: process
- B: fs
- C: http
- D: require

<details><summary><b>Answer</b></summary>

#### Answer: A

All objects that emit events are instances of the EventEmitter class. `process` emit events, so it is an instance of Event Emitter. You can check this via `process instanceof require('events').EventEmitter`.

</details>

###### 12. How can you get the file name(with the directory) that you are working on?

- A: console.log(\_\_dirname)
- B: console.log(filename)
- C: console.log(\_\_filename)
- D: console.log(filename)

<details><summary><b>Answer</b></summary>

#### Answer: C

`console.log(__filename)` will show the file name.

</details>

###### 13. How can you check if a module 'x' exist locally?

- A: require.get(x)
- B: require.resolve(x)
- C: require.find(x)

<details><summary><b>Answer</b></summary>

#### Answer: B

`require.resolve(x)` can give you the full path of the module.

</details>

###### 14. Which one is not a correct property of process(global object)?

- A: .stdin
- B: .title
- C: .clear
- D: .execPath

<details><summary><b>Answer</b></summary>

#### Answer: C

`.clear` is not a property of process.

</details>

###### 15. How can you get absolute path for a specific file app.js?

- A: \_\_filename('app.js')
- B: path.absolute('app.js')
- C: path.resolve('app.js')
- D: \_\_dirname('app.js')

<details><summary><b>Answer</b></summary>

#### Answer: C

`path.resolve('app.js')` will return the absolute path for app.js.

</details>

###### 16. Which method is not a correct method for OS module?

- A: cpus()
- B: platform()
- C: type()
- D: version()

<details><summary><b>Answer</b></summary>

#### Answer: D

`version()` is not a correct method for os module.

</details>

###### 17: Which one is a correct method to create child_process?

- A: fork()
- B: exec()
- C: spawn()
- D: all

<details><summary><b>Answer</b></summary>

#### Answer: D

`all`, there are three ways to create child_process, <b>child_process.exec()</b>, <b>child_process.spawn()</b> & <b>child_process.fork()</b>.

</details>

###### 18: Which DNS method returns an array of record types belonging to the specified hostname?

- A: resolve()
- B: lookupService()
- C: getServers()
- D: lookup()

<details><summary><b>Answer</b></summary>

#### Answer: A

`resolve()`, the resolve function returns an array of record types.

</details>

###### 19: Which object holds arguments pass through a node command?

- A: cli.arguments
- B: process.arguments
- C: process.args
- D: process.argv

<details><summary><b>Answer</b></summary>

#### Answer: D

`process.argv`, holds arguments pass through a node command.

</details>

###### 20: In node 12+, how can you make readFile a promise based method?

- A: const { readFile } = require('fs').promises
- B: const { readFile } = require('fs')
- C: const { readFile } = require('promises')

<details><summary><b>Answer</b></summary>

#### Answer: A

`const { readFile } = require('fs').promises`, by using this you can make readFile a promise based method.

```js
readFile("./file.txt", { encoding: "utf8" })
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

</details>

###### 21: Which one provides Event Loop?

- A: V8
- B: Libuv
- C: C++ bindings

<details><summary><b>Answer</b></summary>

#### Answer: B

Libuv library provides event loop.

</details>

###### 22: APIs of Node.JS are

- A: Asynchronous
- B: Synchronous
- C: Both of the above
- D: None of the above

<details><summary><b>Answer</b></summary>

#### Answer: C

APIs of Node.JS are Asynchronous and Synchronous.

</details>

###### 23: Which module is used to decode Buffer object into strings?

- A: decoder
- B: buffer
- C: string_buffer
- D: string_decoder

<details><summary><b>Answer</b></summary>

#### Answer: D

`string_decoder` is used to decode Buffer object into strings.

</details>

###### 24: Which one is used to expose the node.js modules?

- A: module
- B: module.expose
- C: exports
- D: module.exports

<details><summary><b>Answer</b></summary>

#### Answer: D

Example:

```js
module.exports.bar = "bar";
```

</details>

###### 25: To execute the code of index.js which method should use?

- A: npm index.js
- B: node.index.js
- C: node index.js
- D: npm run index.js

<details><summary><b>Answer</b></summary>

#### Answer: C

`node filepath` Is used to run any javascript file

</details>

###### 26: Which module is used to serve static resources in Node.js?

- A: require
- B: node-resource
- C: fs
- D: node-static

<details><summary><b>Answer</b></summary>

#### Answer: D

You can use `node-static` module to serve static resources. This module is an HTTP static-file server module with built-in caching.

</details>

###### 27: How to install a package (my-package) in node js?

- A: require my-package
- B: node install my-package
- C: npm install my-package
- D: none of the above

<details><summary><b>Answer</b></summary>

#### Answer: C

To install any package in node js just run `npm install package-name` (available in npmjs.com).
example: `npm install my-package`

</details>

###### 28: Which one is used to create and consume custom events?

- A: NodeEvent
- B: EventEmitter
- C: Both of them
- D: none of the above

<details><summary><b>Answer</b></summary>

#### Answer: B

EventEmitter class lies in the events module. It can be accessible like this −

```js
// Import events module
var events = require("events");
// Create an eventEmitter object
var eventEmitter = new events.EventEmitter();
```

</details>

###### 29: Valid form of route path in node.js?

- A: Regular expressions
- B: String
- C: String patterns
- D: All of them

<details><summary><b>Answer</b></summary>

#### Answer: D

You can use String, String pattern and regular expressions to form a route path.

</details>

###### 30: Which module is used to create a server?

- A: fs
- B: http
- C: server
- D: none of the above

<details><summary><b>Answer</b></summary>

#### Answer: B

We use the http instance and call `http.createServer()` method to create a server instance
example:

```js
var http = require("http");
```

</details>

###### 31: Input arguments for an asynchronous queue?

- A: Task function
- B: Concurrency value
- C: Both of them
- D: None of the above

<details><summary><b>Answer</b></summary>

#### Answer: C

Concurrency value and Task function are the main arguments that an asynchronous queue uses.

</details>

###### 32: Which method is used to get the filename part of a file path?

- A: path.basename
- B: path.dirname
- C: path.parse
- D: path.join

<details><summary><b>Answer</b></summary>

#### Answer: A

`path.basename` is user to get the filename part of a file path.

</details>

###### 33: The $ npm ls statement is used to list down all the _____? 

- A: Web application
- B: nodejs sample modules
- C: locally installed modules
- D: package modules

<details><summary><b>Answer</b></summary>

#### Answer: C

The $ npm ls statement is used to list down all the locally installed modules.

</details>

###### 34: Which amongst the following mehtod is used to create instance of http module? 

- A: `var http = require('http');`
- B: `var http = new require('http');`
- C: `var http = new http();`
- D: None of these

<details><summary><b>Answer</b></summary>

#### Answer: A

`var http = require('http');` is the methods of create instance of http module.

</details>

###### 35: The ______ core module is used to create a web server in `Node.js`.

- A: `fs`
- B: `url`
- C: `connect`
- D: `http`

<details><summary><b>Answer</b></summary>

#### Answer: D

The `http` core module is used to create a web server in `Node.js`

</details>

###### 36: Which of the following code gets length of a buffer buf?

- A: buf.length
- B: buf.size
- C: buf.length()
- D: buf.size()

<details><summary><b>Answer</b></summary>

#### Answer: A

`buf.length` returns size of a node buffer in bytes.

</details>

###### 37: Which function is used to include modules in Node Js.

- A: include()
- B: require()
- C: attach()
- D: all

<details><summary><b>Answer</b></summary>

#### Answer: B

`require();` function is used to include modules in Node Js.

</details>

###### 38: Which of the following is a GUI-based debugging tool for Node.js?

- A: Core node debugger
- B: Console
- C: REPL
- D: Node Inspector

<details><summary><b>Answer</b></summary>

#### Answer: D

Node Inspector is a debugger interface for `Node.js` applications that uses the Blink Developer Tools (formerly WebKit Web Inspector).

</details>

###### 39: Which command is used to silence all process warnings including deprecations for app.js?

- A: node app.js --trace-warnings
- B: node app.js --no-deprecation
- C: node app.js --no-warnings
- D: node app.js --trace-deprecation

<details><summary><b>Answer</b></summary>

#### Answer: C

`node app.js --no-warnings` is used to silence all process warnings including deprecations for app.js.

</details>

###### 40: Which method is used to convert path segments into string using the platform-specific separator as a delimiter?

- A: path.join()
- B: path.parse()
- C: path.normalize()
- D: path.format()

<details><summary><b>Answer</b></summary>

#### Answer: A

`path.join()` method joins all given path segments together using the platform-specific separator as a delimiter, then normalizes the resulting path.

</details>

###### 41: Which module is used to take advantage of multi-core systems?

- A: os
- B: dns
- C: stream
- D: cluster

<details><summary><b>Answer</b></summary>

#### Answer: D

`cluster` is used to take advantage of multi-core systems. As node.js runs as single threaded we can take advantage of multi-core systems using cluster module.

</details>

###### 42: Which of the following are Node.js streams types?

- A: writable
- B: transform
- C: readable
- D: all of the above

<details><summary><b>Answer</b></summary>

#### Answer: D

There are four main types of <b>streams</b>` in `Node. js`: `readable`, `writable`, `duplex` and `transform`. Each stream is an eventEmitter instance that emits different events at several intervals.

</details>

###### 43: How to test if two nodes are equal?

- A: isEqualNode()
- B: equal()
- C: ==
- D: None of the above

<details><module><b>Answer</b></module>

#### Answer: A

The Node. `isEqualNode()` method tests whether two nodes are equal.

</details>

###### 44: Third-party packages can be install/update/delete using __. 

- A: Node.exe
- B: Node Package Manager
- C: module.exports
- D: REPL

<details><module><b>Answer</b></module>

#### Answer: B

Third-party packages can be install/update/delete using NPM (Node Package Manager)

</details>

###### 45: When you run JavaScript in a Node.js application, which element in a Node.js stack actually executes that JavaScript?

- A: the libuv library
- B: the VM (like V8 or Chakra)
- C: the c-ares library
- D: the repl module

<details><module><b>Answer</b></module>

#### Answer: B

The VM element will executes when run a Node.js applications.

</details>