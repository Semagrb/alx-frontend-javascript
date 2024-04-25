# Project 0x02: ES6 Classes

Hey there! Welcome to Project 0x02: ES6 Classes. In this project, we'll dive deep into the world of ES6 classes in JavaScript. Let's break down what we're going to cover:

## How to Define a Class

Defining a class in ES6 is pretty straightforward. You start with the `class` keyword followed by the name of your class. Here's a basic example:

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
}
```

In this example, we've defined a class called `Animal` with a constructor method that sets the `name` property of the animal.

## How to Add Methods to a Class

Adding methods to a class is as easy as defining regular functions inside the class. Here's how you can add a method to our `Animal` class:

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}
```

Now our `Animal` class has a `speak` method that logs a message to the console.

## Why and How to Add a Static Method to a Class

Static methods are methods that belong to the class itself, rather than to instances of the class. They are useful for utility functions or operations that don't require an instance of the class. Here's how you can add a static method to our `Animal` class:

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }

  static info() {
    console.log("Animals are awesome!");
  }
}
```

Now you can call the `info` method directly on the `Animal` class without creating an instance.

## How to Extend a Class from Another

Inheritance allows you to create a new class based on an existing class, inheriting its properties and methods. Here's how you can extend the `Animal` class to create a `Dog` class:

```javascript
class Dog extends Animal {
  constructor(name, breed) {
    super(name);
    this.breed = breed;
  }

  fetch() {
    console.log(`${this.name} fetches the ball.`);
  }
}
```

Now the `Dog` class inherits the `speak` method from the `Animal` class and adds its own `fetch` method.

## Metaprogramming and Symbols

Metaprogramming involves writing code that can manipulate itself or other code at runtime. Symbols are a primitive data type introduced in ES6 that can be used as unique property keys. Together, they enable advanced techniques for modifying program behavior dynamically.

That's a wrap for the overview! Let's dive into each topic and start mastering ES6 classes in JavaScript. If you have any questions along the way, feel free to reach out. Happy coding!
