### Control Flow

If a program contains more than one statement - they are executed in an order. The order of execution is in such a way that it tells a story, from top to bottom.

Consider the below snippet :

```js
let myName = "Dtech-Dbug";

console.log("My Name is :" + myName);
//o/p : My Name is :Dtech-Dbug!
```

The above snippet, although hard-coded, really tells a story :

- First we define a variable named `myName`
- Then we print that in the console.

**Note :** Console.log() is a natve binding in JavaScript, a function more specifically. All it does is print anything you pass inbetween the paranthesis onto the console.

A rather simple schematic representation of the above programming would be a top-down arrow.

### Conditional Flows

Not all the time will programs be super simple and a staright and simple top down arrow.
There can(and WILL) very well be cases where the program needs to be branched and the execution needs to follow a certain branch based on the current situation at hand.

Let us consider a real world scenario where branching and execution based on branching occurs.

Imagine you are to buy a particular medicine(for simplicity let us assume that medicine is available in all pharmacies).
The pseudo code will look like :

```
 Get out of House;

 If you find a pharmacy shop;
 Buy the medicine;

 Else Get back home

```
