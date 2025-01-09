# Summary of Typescript

&nbsp;</br>

## What is TypeScript?
TypeScript is an open-source programming language developed by Microsoft. It is a statically typed superset of JavaScript that compiles to plain JavaScript. TypeScript adds optional static typing and other features to JavaScript, making it easier to build large-scale applications while maintaining the flexibility and power of JavaScript.


## Key Features of TypeScript
1.	<b>Static Typing:</b> TypeScript introduces static typing, allowing developers to specify the data types of variables, function parameters, and return values. This helps catch type-related errors during development rather than at runtime.
2.	<b>Interfaces:</b> TypeScript supports interfaces, which define the structure of objects. Interfaces enable better code organization, documentation, and type checking.
3.	<b>Classes:</b> TypeScript includes support for classes, enabling developers to use object-oriented programming concepts such as inheritance, encapsulation, and abstraction.
4.	<b>Enums:</b> Enums allow developers to define a set of named constants, making the code more readable and maintainable.
5.	<b>Generics:</b> TypeScript supports generics, enabling the creation of reusable components that can work with a variety of data types.



## Setting Up TypeScript
To start using TypeScript, you need to install it globally using npm (Node Package Manager):

<code>npm install -g typescript</code>

After installation, you can create a TypeScript file (with a .ts extension) and compile it to JavaScript using the TypeScript compiler (tsc):

<code>tsc yourfile.ts</code>



## Basic TypeScript Syntax
<b>Example 1:</b> 'Hello Github' in TypeScript

``` js
// hello.ts 
	function sayHello(name: string) { 
	console.log("Hello, " + name + "!"); 
	} 
      let user = "John"; 
      sayHello(user); 
```
      
In this example:</br>
•	We define a function 'sayHello' that takes a parameter name of type string.</br>
•	We declare a variable user with the value "John".</br>
•	We call the sayHello function with the user variable as an argument.</br>



<b>Example 2:</b> Static Typing
``` js
// static_typing.ts
let message: string = "Hello, TypeScript!";
let count: number = 10;
let isLogged: boolean = true;

// Error: Type 'number' is not assignable to type 'string'.
message = count;
```

In this example:</br>
•	We explicitly specify the data types of variables message, count, and isLogged.</br>
•	TypeScript detects and reports a type mismatch error when we try to assign a number to a string variable.</br>


<b>Example 3:</b> Interfaces
``` js
// interface.ts
interface Person {
    name: string;
    age: number;
}

function greet(person: Person) {
    return "Hello, " + person.name + ", you are " + person.age + " years old.";
}

let user = { name: "Alice", age: 30 };
console.log(greet(user));
```

In this example:</br>
•	We define an interface Person with properties name and age.</br>
•	We define a function greet that takes an object of type Person as a parameter.</br>
•	We create an object user that conforms to the Person interface and pass it to the greet function.</br>


<b>Example 4:</b> Classes
``` js
// class.ts
class Greeter {
    greeting: string;

    constructor(message: string) {
        this.greeting = message;
    }

    greet() {
        return "Hello, " + this.greeting;
    }
}

let greeter = new Greeter("world");
console.log(greeter.greet());
```

In this example:</br>
•	We define a class Greeter with a property greeting and methods constructor and greet.</br>
•	We create an instance of the Greeter class and call the greet method.</br>



## Conclusion
TypeScript enhances JavaScript by adding static typing, interfaces, classes, enums, generics, and other features. It offers developers the benefits of a statically typed language while preserving the dynamic and flexible nature of JavaScript.


## Further Learning
To deepen your understanding of TypeScript, consider exploring the following resources:
1.	<b>Official TypeScript Documentation:</b> TypeScript Handbook - https://www.typescriptlang.org/docs/handbook/intro.html 
2.	<b>Online Courses:</b> Platforms like Udemy, Coursera, and Pluralsight offer comprehensive TypeScript courses.
3.	<b>Practice Projects:</b> Build small projects using TypeScript to apply your knowledge and improve your skills.
4.	<b>Community Forums:</b> Join TypeScript communities on platforms like Stack Overflow, Reddit, and Discord to ask questions and learn from others.
   




