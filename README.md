# NodeJS Questions

Some common node.js questions and answers.

###### 1. Which one is the node global object?

- A: log
- B: import
- C: process
- D: http

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`process` is one of the node global object. Global objects are globally accessible. These are, <b>__dirname</b>, <b>__filename</b>, <b>module</b>, <b>process</b>, <b>setTimeout</b>, <b>setInterval</b>, <b>setImmediate</b>.

</details>

###### 2. Which module is used to provide compression and decompression functionalities?

- A: net
- B: buffer
- C: zlib
- D: dns

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`zlib` module provides compression(zip) and decompression(unzip) functionalities.

</details>

###### 3. Which console method is used to show the stack trace?

- A: stack
- B: log
- C: trace
- D: debug

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`trace` method is used to show the stack trace.

</details>

###### 4. Which module would you use to get the server information?

- A: dns
- B: url
- C: net
- D: tls

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

`dns` module is used to get the server information.

</details>

###### 5. Which one is used to read a file asynchronously?

- A: fs.getFile
- B: fs.read
- C: fs.readFile
- D: fs.get

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`fs.readFile` is used to read a file asynchronously.

</details>

###### 6. Which module would you use to encrypt data?

- A: crypto
- B: process
- C: encrypt

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

`crypto` module is used to encrypt data.

</details>

###### 7. Which method is used to exit(kill) in node.js?

- A: kill
- B: exit
- C: stop

<details><summary><b>Answer</b></summary>
<p>

#### Answer: B

`process.exit()` is used to exit in node.js.

</details>

###### 8. Which one is the core module of node?

- A: require
- B: import
- C: fs
- D: process

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`fs` is a core module of node. Some of them are, <b>buffer</b>, <b>crypto</b>, <b>dns</b> etc.

</details>

###### 9. Which command is used to tell node to run javascript strict mode in node repl?

- A: node -strict
- B: node --strict
- C: node --use-strict
- D: node -use--strict

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`node --use-strict` will run node in javascript strict mode.

</details>

###### 10. Which one is not a node repl command?

- A: .save
- B: .clear
- C: .help
- D: .find

<details><summary><b>Answer</b></summary>
<p>

#### Answer: D

`.find` is not a node repl command. The repl commands are, <b>.break</b>, <b>.clear</b>, <b>.editor</b>, <b>.exit</b>, <b>.help</b>, <b>.load</b>, <b>.save</b>.

</details>

###### 11. Which one is an instance of Event Emitter?

- A: process
- B: fs
- C: http
- D: require

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

All objects that emit events are instances of the EventEmitter class. `process` emit events, so it is an instance of Event Emitter. You can check this via `process instanceof require('events').EventEmitter`.

</details>

###### 12. How can you get the file name(with the directory) that you are working on?

- A: console.log(__dirname)
- B: console.log(filename)
- C: console.log(__filename)
- D: console.log(filename)

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`console.log(__filename)` will show the file name.

</details>

###### 13. How can you check if a module 'x' exist locally?

- A: require.get(x)
- B: require.resolve(x)
- C: require.find(x)

<details><summary><b>Answer</b></summary>
<p>

#### Answer: B

`require.resolve(x)` can give you the full path of the module.

</details>

###### 14. Which one is not a correct property of process(global object)?

- A: .stdin
- B: .title
- C: .clear
- D: .execPath

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`.clear` is not a property of process.

</details>

###### 15. How can you get absolute path for a specific file app.js?

- A: __filename('app.js')
- B: path.absolute('app.js')
- C: path.resolve('app.js')
- D: __dirname('app.js')

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

`path.resolve('app.js')` will return the absolute path for app.js.

</details>

###### 16. Which method is not a correct method for OS module?

- A: cpus()
- B: platform()
- C: type()
- D: version()

<details><summary><b>Answer</b></summary>
<p>

#### Answer: D

`version()` is not a correct method for os module.

</details>

###### 17: Which one is a correct method to create child_process?

- A: fork()
- B: exec()
- C: spawn()
- D: all

<details><summary><b>Answer</b></summary>
<p>

#### Answer: D

`all`, there are three ways to create child_process, <b>child_process.exec()</b>, <b>child_process.spawn()</b> & <b>child_process.fork()</b>.

</details>

###### 18: Which DNS method returns an array of record types belonging to the specified hostname?

- A: resolve()
- B: lookupService()
- C: getServers()
- D: lookup()

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

`resolve()`, the resolve function returns an array of record types.

</details>

###### 19: Which object holds arguments pass through a node command?

- A: cli.arguments
- B: process.arguments
- C: process.args
- D: process.argv

<details><summary><b>Answer</b></summary>
<p>

#### Answer: D

`process.argv`, holds arguments pass through a node command.

</details>

###### 20: In node 12+, how can you make readFile a promise based method?

- A: const { readFile } = require('fs').promises
- B: const { readFile } = require('fs')
- C: const { readFile } = require('promises')

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

`const { readFile } = require('fs').promises`, by using this you can make readFile a promise based method.

```js
readFile('./file.txt', { encoding: 'utf8' })
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

</details>