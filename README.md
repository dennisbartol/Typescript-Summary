# Introduction to Typescript


# What is TypeScript?
TypeScript is an open-source programming language developed by Microsoft. It is a statically typed superset of JavaScript that compiles to plain JavaScript. TypeScript adds optional static typing and other features to JavaScript, making it easier to build large-scale applications while maintaining the flexibility and power of JavaScript.


# Key Features of TypeScript
1.	<b>Static Typing:</b> TypeScript introduces static typing, allowing developers to specify the data types of variables, function parameters, and return values. This helps catch type-related errors during development rather than at runtime.
2.	<b>Interfaces:</b> TypeScript supports interfaces, which define the structure of objects. Interfaces enable better code organization, documentation, and type checking.
3.	<b>Classes:</b> TypeScript includes support for classes, enabling developers to use object-oriented programming concepts such as inheritance, encapsulation, and abstraction.
4.	<b>Enums:</b> Enums allow developers to define a set of named constants, making the code more readable and maintainable.
5.	<b>Generics:</b> TypeScript supports generics, enabling the creation of reusable components that can work with a variety of data types.



# Setting Up TypeScript
To start using TypeScript, you need to install it globally using npm (Node Package Manager):

<code>npm install -g typescript</code>

After installation, you can create a TypeScript file (with a .ts extension) and compile it to JavaScript using the TypeScript compiler (tsc):

<code>tsc yourfile.ts</code>



# Basic TypeScript Syntax
<b>Example 1:</b> 'Hello Github' in TypeScript

<code>// hello.ts 
	function sayHello(name: string) { 
	console.log("Hello, " + name + "!"); 
	} 
      let user = "John"; 
      sayHello(user); 
</code>
      
In this example:</br>
•	We define a function 'sayHello' that takes a parameter name of type string.</br>
•	We declare a variable user with the value "John".</br>
•	We call the sayHello function with the user variable as an argument.</br>



<b>Example 2:</b> Static Typing
<code>
// static_typing.ts
let message: string = "Hello, TypeScript!";
let count: number = 10;
let isLogged: boolean = true;

// Error: Type 'number' is not assignable to type 'string'.
message = count;
</code>

In this example:</br>
•	We explicitly specify the data types of variables message, count, and isLogged.</br>
•	TypeScript detects and reports a type mismatch error when we try to assign a number to a string variable.</br>


<b>Example 3:</b> Interfaces
<code>
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
</code>

In this example:</br>
•	We define an interface Person with properties name and age.</br>
•	We define a function greet that takes an object of type Person as a parameter.</br>
•	We create an object user that conforms to the Person interface and pass it to the greet function.</br>



