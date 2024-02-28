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
Example 1: 'Hello Github' in TypeScript

<code>// hello.ts function sayHello(name: string) { 
	console.log("Hello, " + name + "!"); 
	} 
      let user = "John"; sayHello(user); 
</code>
      
In this example:
•	We define a function sayHello that takes a parameter name of type string.</br>
•	We declare a variable user with the value "John".</br>
•	We call the sayHello function with the user variable as an argument.</br>


