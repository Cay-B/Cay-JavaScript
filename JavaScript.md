# JavaScript

- **Variables**
    
    ## Let & **Const**
    
    Const variables are variables that can't be reassigned, while let variables cab be reassigned 
    
    **Example (let)**
    
    **let x = 3**
    
    **console.log(x)**
    
    **// output: 3**
    
    **let x = 5**
    
    **console.log(x)**
    
    **// output: 5**
    
    **Example (const)** 
    
    **const name = “Cay”**
    
    **console.log(name)**
    
    **// output: Cay**
    
    **const name = “armond”**
    
    **console.log(name)**
    
    **// output: error**
    
- **Data types**
    
    ## Data Types in JavaScript
    
    JavaScript has several built-in data types, including:
    
    - **Numbers**: Used for numeric values, including integers and decimals.
        
        **const age = 21**
        
    - **Strings**: Used for textual data, which can be enclosed in single or double quotes.
        
        **let name = “Cay”**
        
    - **Booleans**: Used for logical values, which can be either `true` or `false`.
        
        **const isSunny = True**
        
    - **Undefined**: Used to indicate a variable that has not been assigned a value.
    - **const x = Undefined**
    - **Null**: Used to indicate that a variable has been intentionally assigned no value.
        
        **const num = null**
        
    - **Objects**: Used to represent more complex data structures, such as arrays and key-value pairs.
    - **Symbols**: Used to represent unique identifiers for objects or properties.
    
    JavaScript also has a dynamic data type system, which means that variables can be reassigned to different data types at any time.
    
- **Arrays**
    
    ## Arrays
    
    Arrays are a type of data structure in JavaScript used for storing and organizing multiple values. They are declared using square brackets and can contain any number of values, separated by commas.
    
    ```
    const fruits = ['apple', 'banana', 'orange'];
    console.log(fruits); // output: ['apple', 'banana', 'orange']
    
    ```
    
    You can access specific elements in an array by using their index number, which starts at 0 for the first element.
    
    ```
    const fruits = ['apple', 'banana', 'orange'];
    console.log(fruits[0]); // output: 'apple'
    
    ```
    
    You can also add or remove elements from an array using various methods, such as `push()`, `pop()`, `shift()`, and `unshift()`.
    
    ```
    const fruits = ['apple', 'banana', 'orange'];
    fruits.push('pear'); // adds 'pear' to end of array
    console.log(fruits); // output: ['apple', 'banana', 'orange', 'pear']
    
    fruits.pop(); // removes last element from array
    console.log(fruits); // output: ['apple', 'banana', 'orange']
    
    ```
    
- **Data structures**
    
    ## Data Structures
    
    JavaScript has several built-in data structures, including:
    
    - **Arrays**: Used for storing and organizing multiple values using numeric indexes.
    - **Objects**: Used for storing and organizing more complex data structures using key-value pairs.
    - **Maps**: Used for storing key-value pairs where the keys can be of any data type.
    - **Sets**: Used for storing unique values of any data type.
    - **WeakMaps**: Similar to maps, but with weaker object reference semantics.
    - **WeakSets**: Similar to sets, but with weaker object reference semantics.
    
    Each of these data structures has its own unique features and use cases, and can be used in a variety of ways to store and manipulate data in JavaScript.
    
- **Session and local storage**
    
    ## Session and Local Storage
    
    Session storage and local storage are two JavaScript objects that allow you to store key-value pairs in the client's web browser. They are similar in functionality, but differ in their storage duration and scope.
    
    ### Session Storage
    
    Session storage is used to store data that should only be available for the duration of the current browser session. This means that the data will be cleared when the user closes the browser window or tab. To store data in session storage, you can use the `sessionStorage` object.
    
    ```
    // Store data in session storage
    sessionStorage.setItem('username', 'john');
    
    // Retrieve data from session storage
    const username = sessionStorage.getItem('username');
    console.log(username); // output: 'john'
    
    // Remove data from session storage
    sessionStorage.removeItem('username');
    
    ```
    
    ### Local Storage
    
    Local storage is used to store data that should persist beyond the current browser session. This means that the data will continue to be available even after the user closes the browser window or tab. To store data in local storage, you can use the `localStorage` object.
    
    ```
    // Store data in local storage
    localStorage.setItem('username', 'john');
    
    // Retrieve data from local storage
    const username = localStorage.getItem('username');
    console.log(username); // output: 'john'
    
    // Remove data from local storage
    localStorage.removeItem('username');
    
    ```
    
    It's important to note that both session storage and local storage have a limit on the amount of data you can store, which varies by browser. Additionally, you should be cautious about storing sensitive data in these objects, as they can be accessed by JavaScript code running on the same page.
    
- **Conditional statement**
    
    ## Conditional Statements
    
    In JavaScript, conditional statements are used to execute different actions based on different conditions. The most common conditional statements in JavaScript are `if`, `else`, and `else if`. These statements are used to check if a certain condition is true, and execute specific code blocks accordingly.
    
    ### If Statement
    
    The `if` statement is used to check if a certain condition is true, and execute a specific code block if it is. The basic syntax of an `if` statement is as follows:
    
    ```
    if (condition) {
      // Code block to be executed if the condition is true
    }
    
    ```
    
    Here's an example:
    
    ```
    let x = 10;
    if (x > 5) {
      console.log("x is greater than 5");
    }
    
    ```
    
    In this example, the condition `x > 5` is true, so the code block inside the `if` statement will be executed, and the output will be `x is greater than 5`.
    
    ### Else Statement
    
    The `else` statement is used in conjunction with the `if` statement, and is executed if the `if` statement's condition is false. The basic syntax of an `if/else` statement is as follows:
    
    ```
    if (condition) {
      // Code block to be executed if the condition is true
    } else {
      // Code block to be executed if the condition is false
    }
    
    ```
    
    Here's an example:
    
    ```
    let x = 3;
    if (x > 5) {
      console.log("x is greater than 5");
    } else {
      console.log("x is less than or equal to 5");
    }
    
    ```
    
    In this example, the condition `x > 5` is false, so the code block inside the `else` statement will be executed, and the output will be `x is less than or equal to 5`.
    
    ### Else If Statement
    
    The `else if` statement is used in conjunction with the `if` statement, and allows for multiple conditions to be checked. The basic syntax of an `if/else if/else` statement is as follows:
    
    ```
    if (condition1) {
      // Code block to be executed if condition1 is true
    } else if (condition2) {
      // Code block to be executed if condition1 is false and condition2 is true
    } else {
      // Code block to be executed if both condition1 and condition2 are false
    }
    
    ```
    
    Here's an example:
    
    ```
    let x = 0;
    if (x > 0) {
      console.log("x is positive");
    } else if (x < 0) {
      console.log("x is negative");
    } else {
      console.log("x is zero");
    }
    
    ```
    
    In this example, the condition `x > 0` is false, so the `if` statement is skipped. The `else if` statement's condition `x < 0` is also false, so the `else` statement is executed, and the output will be `x is zero`.
    
- **Loops**
    
    Loops are used in JavaScript to perform repeated tasks based on a condition. Conditions typically return `true` or `false`. A loop will continue running until the defined condition returns `false`**.**
    
    ### **`for` Loop**
    
    ### **Syntax**
    
    ```
    for (initialization; condition; finalExpression) {
      // code
    }
    
    ```
    
    The `for` loop consists of three optional expressions, followed by a code block:
    
    - `initialization` - This expression runs before the execution of the first loop, and is usually used to create a counter.
    - `condition` - This expression is checked each time before the loop runs. If it evaluates to `true`, the `statement` or code in the loop is executed. If it evaluates to `false`, the loop stops. And if this expression is omitted, it automatically evaluates to `true`.
    - `finalExpression` - This expression is executed after each iteration of the loop. This is usually used to increment a counter, but can be used to decrement a counter instead.
    
    Any of these three expressions or the the code in the code block can be omitted.
    
    `for` loops are commonly used to run code a set number of times. Also, you can use `break` to exit the loop early, before the `condition` expression evaluates to `false`.
    
    Example: 
    
    ```
    for(let i = 0; i < 5; i++){
    console.log(i)
    }
    
    // output:
    // 0
    // 1
    // 2
    // 3
    // 4
    ```
    
    ### **`while` Loop**
    
    ### **Syntax**
    
    ```
    while (condition) {
      // statement
    }
    
    ```
    
    The `while` loop starts by evaluating `condition`. If `condition` evaluates to `true`, the code in the code block gets executed. If `condition` evaluates to `false`, the code in the code block is not executed and the loop ends.
    
    ```
    let i = 0;
    
    while (i < 5) {
      console.log(i);
      i++;
    }
    
    // Output:
    // 0
    // 1
    // 2
    // 3
    // 4
    ```
    
    ### **`do...while` loop**
    
    ### **Syntax:**
    
    ```
    do {
      // statement
    } while (condition);
    
    ```
    
    The `do...while` loop is closely related to `while` loop. In a `do...while` loop, `condition` is checked at the end of each iteration of the loop, rather than at the beginning before the loop runs.
    
    This means that code in a `do...while` loop is guaranteed to run at least once, even if the `condition` expression already evaluates to `true`.
    
    ```jsx
    let i = 0;
    
    do {
      console.log(i);
      i++;
    }
    while (i < 5)
    
    // Output:
    // 0
    // 1
    // 2
    // 3
    // 4
    ```
    
- **Objects**
    
    ## Objects
    
    Objects are a data type in JavaScript used for storing and organizing more complex data structures. They are similar to arrays, but instead of using numeric indexes, object properties are accessed using keys.
    
    Objects are declared using curly braces, and properties are defined using key-value pairs, separated by colons.
    
    ```
    const person = {
      name: "Cay",
      age: 21,
      email: "olompus71@gmail.com"
    };
    
    ```
    
    You can access specific properties in an object using dot notation or bracket notation.
    
    ```
    const person = {
      name: "Cay",
      age: 21,
      email: "olompus71@gmail.com"
    };
    
    console.log(person.name); // output: "Cay"
    console.log(person["age"]); // output: 21
    
    ```
    
    You can also add or remove properties from an object using dot notation or bracket notation.
    
    ```
    const person = {
      name: "Cay",
      age: 21,
      email: "olompus71@gmail.com"
    };
    
    person.phone = "+251933366206"; // adds a new property
    console.log(person); // output: {name: "Cay", age: 21, email: "olompus71@gmail.com", phone: "+251933366206"}
    
    delete person.email; // removes a property
    console.log(person); // output: {name: "Cay", age: 21, phone: "+251933366206"}
    
    ```
    
- **Functions**
    
    ## Function Declaration
    
    To create a function we can use a *function declaration*.
    
    It looks like this:
    
    `function showMessage() {
      alert( 'Hello everyone!' );
    }`
    
    The `function` keyword goes first, then goes the *name of the function*, then a list of *parameters* between the parentheses (comma-separated, empty in the example above, we’ll see examples later) and finally the code of the function, also named “the function body”, between curly braces.
    
    `function name(parameter1, parameter2, ... parameterN) {
     // body
    }`
    
    Our new function can be called by its name: `showMessage()`.
    
    For instance:
    
    `function showMessage() {
      alert( 'Hello everyone!' );
    }
    
    *showMessage();
    showMessage();*`
    
    The call `showMessage()` executes the code of the function. Here we will see the message two times.
    
    This example clearly demonstrates one of the main purposes of functions: to avoid code duplication.
    
    If we ever need to change the message or the way it is shown, it’s enough to modify the code in one place: the function which outputs it.
    
    ## Function Naming
    
    Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.
    
    It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.
    
    For instance, functions that start with `"show"` usually show something.
    
    Function starting with…
    
    - `"get…"` – return a value,
    - `"calc…"` – calculate something,
    - `"create…"` – create something,
    - `"check…"` – check something and return a boolean, etc.
    
    Examples of such names:
    
    `showMessage(..)     // shows a message
    getAge(..)          // returns the age (gets it somehow)
    calcSum(..)         // calculates a sum and returns the result
    createForm(..)      // creates a form (and usually returns it)
    checkPermission(..) // checks a permission, returns true/false`
    
    With prefixes in place, a glance at a function name gives an understanding what kind of work it does and what kind of value it returns.
    
- **Event Listener**
    
    The JavaScript addEventListener() method allows you to set up functions to be called when a specified event happens, such as when a user clicks a button. This tutorial shows you how you can implement addEventListener() in your code.
    
    ## ****addEventListener() Syntax****
    
    ```jsx
    target.addEventListener(event, function, useCapture)
    ```
    
    - **target**: the HTML element you wish to add your event handler to. This element exists as part of the Document Object Model (DOM) and you may wish to learn about [how to select a DOM element](https://1000mileworld.com/dom-manipulation-using-javascript/#select).
    - **event**: a string that specifies the name of the event. We already mentioned `load` and `click` events. For the curious, here's a full list of [HTML DOM events](https://www.w3schools.com/jsref/dom_obj_event.asp).
    - **function**: specifies the function to run when the event is detected. This is the magic that can allow your web pages to change dynamically.
    - **useCapture**: an optional Boolean value (true or false) that specifies whether the event should be executed in the [capturing or bubbling phase](https://javascript.info/bubbling-and-capturing). In the case of nested HTML elements (such as an `img` within a `div`) with attached event handlers, this value determines which event gets executed first. By default, it's set to false which means that the innermost HTML event handler is executed first (bubbling phase).
    
    **Example**
    
    ```
    let button = document.querySelector('#button');
    let msg = document.querySelector('#message');
    
    button.addEventListener('click', ()=>{
      msg.classList.toggle('reveal');
    })
    ```
    
    ## ****Passing Event as a Parameter****
    
    ```
    button.addEventListener('click', (e)=>{
      console.log(e.target.id)
    })
    ```
    
    ## ****Removing Event Handlers****
    
    ```
    target.removeEventListener(event, function, useCapture);
    
    ```
    
    The parameters are the same as `addEventListener()`.
    
- **DOM**
    - **What is DOM**
        
        The ***Document Object Model (DOM)*** is an application programming interface (API) for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can interact with the page.
        
    - **The Nature & Function of DOM**
        
        In the DOM, everything is a node. The document itself is a document node. Some other examples of nodes are element nodes and attribute nodes. Element nodes represent HTML elements. Element nodes can have attributes, such as the id or class attribute, that programmers can interact with using the DOM.
        
        Attribute nodes are part of element nodes. An element node can have multiple attributes, and each attribute is a separate node.
        
        Using the DOM, programmers can create, delete, and change elements, attributes, and text nodes. For example, to add a new HTML element to a page:
        
        1. Create the element using the `createElement` method.
        2. Create the text for the element using the `createTextNode` method.
        3. Add the text to the element using the `appendChild` method.
        4. Add the element to the document using the `appendChild` method.
        
        The DOM also provides methods and properties to access and manipulate styles and classes, handle events, and create animations.
        
    - **DOM Example**
        
        
        Here's an example of using the DOM in JavaScript to change the text of an HTML element with the id "example":
        
        ```
        // Get the element with the id "example"
        var example = document.getElementById("example");
        
        // Change the text of the element
        example.textContent = "New text";
        
        ```
        
        In this example, we first use the `getElementById` method to select the HTML element with the id "example". Then, we use the `textContent` property to change the text of the element to "New text".
        
    - **Conclusion**
        
        Overall, the DOM is a powerful tool for web developers to create dynamic and interactive web pages using programming languages like JavaScript.