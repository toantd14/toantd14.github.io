# Compare Tech

## Specification Language
1. [Server-side I/O Performance: Node vs. PHP vs. Java vs. Go](https://www.toptal.com/back-end/server-side-io-performance-node-php-java-go)

    Language | Threads vs. Processes | Non-blocking I/O | Ease of Use
    --|--|--|--
    PHP | Processes | No | |
    Java | Threads | Available | Requires Callbacks
    Node.js | Threads | Yes | Requires Callbacks
    Go | Threads (Goroutines) | Yes | No Callbacks Needed

2. [Process vs Thread](https://www.educba.com/process-vs-thread/)

    Process|Thread
    --|--
    An instance of a program to execute is called process.|Threads are the subset of the process and run within the process.
    The address space is not shared by the process to improve security. Each process has a separate virtual address space.|The address space is shared by the threads within the process that is virtually allocated logical space.
    The files of different processes cannot be accessed together as it has different address space.|All the files of different threads of the same process can be accessed together due to the shared address space.
    Registers are not at all required by the process to execute the program.|Separate registers for each thread are required to function.
    Accounting information is needed by the process to save all the information of the program and check for discrepancies.|Accounting information is not needed in threads as all the information belongs to the process, and it is captured already.
    Stacks and state are not needed per process as the codes are taken care of by the threads, and the information related are stored.|Stacks and states are needed per threads for the execution of the codes in the process.
    Global variables define the process in the scenario of describing the program and is needed while executing the program.|Global variables are not needed in the threads as it is not known without the process they represent.
    There are child processes for the main process, which is executed one after the other.|There are no child threads for the threads in the process. There can only be different threads for the process.
    Signal handlers are needed in the process to direct the traffic of codes and to allocate the memory space.|Since threads are a subset of process, signal handlers are not needed in threads.
    The process has a complete set of its own resources to do the tasks allocated, and hence it is in a contained environment.|Threads share the resources of processes to do the task, which may result in communication problems.
    When we open word and PowerPoint in a system, this is called two processes.|In a word, while editing the document, saving happens simultaneously. This is because editing and saving are happening in two threads.
    The process will never do the tasks of another process. This results in crashing the application and can never be done so.|Any part of the code in the process is executed by the thread. This includes the codes being executed by other threads as well.
    The fork () method is used to create the process. Fork is the procedure of copying the files by keeping the original files.|Clone() method is used to create the thread. Clone is the method of copying files without keeping the original files in space.
    The process takes time to switch between contexts.|While comparing with the process, context switching does not take much time in threads.

3. [Golang vs Node.js vs PHP vs Python vs Ruby](https://www.npmtrends.com/golang-vs-node.js-vs-php-vs-python-vs-ruby)


## Socket.io vs Websockets vs REST
### Socket.io vs Websockets
1. [WebSocket vs Socket.io](https://www.educba.com/websocket-vs-socket-io/)
2. [Differences between socket.io and websockets](https://stackoverflow.com/a/38558531/17609935)
3. [Sự khác nhau giữa socket.io và websockets?](https://helpex.vn/question/su-khac-nhau-giua-socket.io-va-websockets-5cb1673aae03f6169c9e584e)

    #|Socket.io|WebSocket
    --|--|--
    1| It is the library to work with WebSocket|It is the protocol that is established over the TCP connection
    2|Provides the event-based communication between browser and server|It provides full-duplex communication on TCP connections
    3|A connection can be established in the presence of proxies and load balancers|Proxy and load balancer is not supported in WebSocket
    4|It supports broadcasting|It doesn’t support broadcasting
    5|It supports fallback options|It doesn’t have a fallback option

### Socket.io vs REST
1. [WebSocket vs REST](https://www.educba.com/websocket-vs-rest/)
2. [WebSockets vs REST: Understanding the Difference](https://www.pubnub.com/blog/websockets-vs-rest-api-understanding-the-difference/)

    #|Socket.io|REST
    --|--|--
    HTTP|Use of HTTP occur in initial connection|HTTP is common protocal in RESRful web services
    Communication|Bi-directional in nature.|Uni-directional in nature.
    Nature|Socket-based concept.|Resources based concept, rather than commands.
    Scenario|Real-time chat application.|Lots of getting request.
    Dependency|Rely on IP address and port number.|Based on the HTTP protocol and uses HTTP methods to relay data.
    Cost|The cost of communication is lower.|The cost of communication is comparatively higher than WebSocket.
    Performance|Better with high loads.|Great for occasional communication.
    State|WebSocket is a stateful protocol.|REST is based on HTTP, which is a stateless protocol.


## API Protocol Standard
1. [So Sánh Các Chuẩn Giao Thức API: SOAP vs REST vs GraphQL vs RPC](https://www.facebook.com/grokking.vietnam/photos/a.785503414850962/3896533527081253/)
2. [Một vài liên hệ giữa Web APIs, WebSocket và HTTP](https://medium.com/old-dev/m%E1%BB%99t-v%C3%A0i-li%C3%AAn-h%E1%BB%87-gi%E1%BB%AFa-web-apis-websocket-v%C3%A0-http-b4850804c1d0)

    #|RPC|SOAP|REST|GraphQL
    --|--|--|--|--
    Organized in terms of|local procedure calling|enveloped message structure|compliance with six architectural constraints|schema & type system
    Format|JSON, XML, Protobuf, Thrift, FlatBuffers|**XML only**|XML, SJON, HTML, plain text|JSON
    Learning curve|**Easy**|**Difficult**|**Easy**|**Medium**
    Community|**Large**|**Small**|**Large**|**Growing**
    Use cases|Command and action-oriented APIs; internal high perfomance communication in massive micro-services systems|Payment gateways, identity management CRM solution financial and telecommunication services, legacy system support|Puclic APIs simple resource-driven apps|Mobile APIs complex systems, micro-services

## Compare Other
### Typescript vs ES6

1. [TypeScript vs JavaScript](https://www.educba.com/typescript-vs-javascript/)

    #|Typescript|Javascript
    --|--|--
    Type|Typescript is a strongly type object-oriented compile language|JavaScript is a lightweight,     interpreted programming language
    Design & Developed by|As already explained above, it was designed and developed by Anders Hejlsberg at Microsoft.|Brendan Eich at Netscape Communications Corporation, Mozilla Foundation, ECMA International.
    Light/Heavy Weight|It is heavy weighted. an interpreted programming language.|It is a light weighted It is specially designed for development of large application and trans compile to JavaScript
    Client Side/ Server Side|Specially used in Client Side|Both client-side and server-side
    File Extension|. ts, .tsx|.js
    Syntax|Syntax defines a set of rules for writing programs.Every language specification defines its own syntax. A Typescript program is composed of (Modules, Functions, Variables, Statements and Expressions Comments)|In JavaScript, all the statements are written within Script tagIt tells the browser program to start interpreting all the text between these tags as a script
    Benefits||
    Preference to choose|Since Typescript is an object-oriented language. Which makes our code more consistent, clean, simple and reusable. So it should better to use typescript for developing large projects.|JavaScript is preferable to use in relatively small coding projects.



2. [Typescript vs ES6](https://www.educba.com/typescript-vs-es6/)

    #|Typescript|ES6
    --|--|--
    Definition|Typescript is to eradicate the development errors|ES6 is comparatively more flexible in development time
    Explanation|TypeScript is a free and open-source programming language. It is developed and maintained by Microsoft.|ES6 is a version of ECMAScript (ES), which is a scripting language specification standardized by ECMA international.
    Benefits|TypeScript supports all primitive data types|ES6 will not support.
    Variables|Typescript having 3 scopes (Global Scope, Class Scope, Local Scope)|ES6 having 2 scopes (Global Scope, Local Scope)
    Decision-Making|1.if Statement + 2.if-else Statement + 3.else…if and nested if statements + 4.switch Statement|1.if Statement + 2.if-else Statement + 3.The else- if ladder/nested if statements + 4.switch–case Statement
    Modules|Modules are of 2 types of Internal and external modules|In ES6, modules are classified as importing a module and exporting a module.
    Loops|Typescript and ES6 both are having the same loops (Definite, Indefinite)|Typescript and ES6 both are having the same loops (Definite, Indefinite)

3. [ES6 vs ES5](https://www.educba.com/es6-vs-es5/)

    #|ES6|ES5
    --|--|--
    Definition|ECMA script is basically a trademarked scripting language specification defined by Ecma international. The sixth edition of the same is known as ES6.|ECMA script is a trademarked scripting language specification defined by Ecma international. The fifth edition of the  same is known as ES5.
    Using Arrow Functions|In the case of ES6, the function keyword need not be used to define the function and also, the return keyword can be avoided to fetch the computed value.|In the case of ES5, function and return, both keywords need to be used to define the functions.
    Object Manipulation|Object manipulation can be processed more smoothly in ES6 (due to the presence of destructuring, speed operators) than in its previous versions.|ES5 also provides the same features, but it’s a bit more time consuming than that of ES6.
    Performance|With the help of newly implemented features and shorthand storage implementation, ES6 scores a higher performance rank than ES5.|ES5 is the prior version to ES6, and thus, due to the non-presence of a few features, its performance is a bit less than that of ES6
    Support|There is also a lot of community support for ES6. However, it is lesser than that of ES5.|ES5 provide a larger range of community supports than that of ES6

4. [Encryption vs Decryption](https://www.educba.com/encryption-vs-decryption/)

    Aspect|Encryption|Decryption
    --|--|--
    Definition|Encryption is the procedure to convert normal data into a form that is unreadable. It helps us to prevent any sort of unauthorized access to the data.|Decryption is the procedure to convert unreadable or encrypted data into its original or normal form.
    Procedure|The data is encrypted/coded automatically with the help of a secret key when data is being transferred between two different machines.|The data receiver lets you to automatically decipher the code in its actual form using the data that was sent.
    Conversion Location|The sender, while sending the data to the destination, will convert it.|The receiver, while receiving the data, would convert it.
    Instance|The employee, while sending a few critical documents to their managers.|The manager, while receiving a few critical documents from their employees.
    Algorithm|The algorithm and the key that is used is the same for the encryption-decryption process.|Two keys where each one is used for encryption and then decryption.
    Functionality/Use|To transform easily understandable and human decipherable messages into a non – decipherable and obscure form that is almost incomprehensible to interpret.|It is the transformation of an obscure message into a decipherable form that is understood by a human.

