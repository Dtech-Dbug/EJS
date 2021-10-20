## Program Structures

#### Expressions

- Every block/line of code that produces a value is called an expression.
- Every value written literally like 'Programmer' or 'JavaScript' or any numerics like 2 is an expression.
- An Expression within a parenthesis (expression) is also an expression.
- Unary or Binary Operations involving expressions is also an expression.

This is the beauty of language based interface - as most of English can be directly used in logic formation and deductions.

Consider the following example below :

> If the program has bugs or the program involves division by 0. The program will crash.

This is an excellent example of the beauty of language based interface. The above example is really comprised of two sentences :

- If the program has bugs

  **OR**

- If the program involves division by 0

We used two sub sentences to form a single sentence - and similarly two sub expressions to form a single expression.

The above example is essentially a _conditional statement_, in the form of `if(p or q) then r`.
Where p , q, r are just statement variables which can be substituted by actual english.

**_If an expression corresponds to a sentence fragment, a JavaScript statement corresponds to a full sentence. A program is a list of statements._**

**Note :** A statement is an expression that has a consistent truth value. i.e, it can either be true or false but never both. On the contrary, a sentence is an expression that bears inconsistent truth values meaning for some cases it may be true and other cases false.

---

#### Statements

We introduced the fundamenetals of statements just a few lines ago.
The simplest statement in programming paradigm is an expression that ends with a semi-colon.

Example :

```js

Hello World;
!false;

```

That is it. That is a statement. Although very trivial and useless admittedly, but does not change the fact that the above lines are two statements.

🎯 **A statement only amounts to something when it affects the environment(in context of the program scope). It could be something as simple as printing something on the console or updating a variable which is then used by some other block of code. Either cases the statements are likely to affect the program and it's state. These changes and similar changes alike are called _SIDE EFFECTS_ .**

**Note:** JavaScript is lineant sometimes and ignores missing semi-colons in certain cases. But the best practise would be to use them - in order to ignore the nuances of missing terminating characters.

---

### How does JavaScript keep an internal state or remember values? 🤔

To catch and hold values, JavaScript uses something called **Bindings** or simply variables.
Consider the snippet below :

```js
let Greet = "Hello World, JavaScript is amazing!";
```

The above line is literally indicating a binding and it is another kind of statement.

- The special keyword `let` indicates that the sentence is going to define a binding.
  (More about these special keywords, soon)

- Followed by the name of the binding.

- And we immediately assigned a value to the binding by using the `=` and an expression, which is `Hello World, JavaScript is amazing!`

**Note:** `=` in programming is assignment operator. Not equality operator!

By the example statement - it creates a binding called Greet to point towards the value `Hello World, JavaScript is amazing!`

When a binding points towards a value - it does not essentially gets tied to it forever.
Meaning, that at any point of time, we can use the `=` operator again on existing bindings to make it point towards a new value.

Continuation of the previous example :

```js
let Greet = "Hello Reader";

let Question = "How are you liking JavaScript?";
```

As obvious as it seems - we made the binding named _Greet_ point to a new value now. And also defined a new binding named _Question_.

When bindings are defined, we can use their names as expressions. Example :

```js
let Greet = "Hello Reader";

let Question = "How are you liking JavaScript?";

let Welcome = Greet + Question;

// the binding named welcome will hold the value "Hello Reader How are you liking JavaScript?"
```

The above example may seem a little cryptic if you are an absolute beginner to programming. But what it is doing essentially is just concatanateing two strings because we used an expression that includes a binary operation between two expressions `Greet + Question`

Consider a simple example for usage of defined bindings as expressions.
Imagine Santa Clause 🎅 gives you 1000$ on Christmas and again 2000$ on New Year's eve.
The equivalent code will look like :

```js
let FirstGiftBySanta = 1000;

let SecondGiftBySanta = FirstGiftBySanta + 2000;

console.log(SecondGiftBySanta);
//output : 3000 (1000 + 2000)
```

_When you define a binding, and do not assign it any value to point at, it ends up pointing to a bogus address. HEnce if you try to retrieve the value of such a binding you are likely to see `undefined`_

But, you can assign a value to it later in your code. Example :

```js
let LuckyNumber;

LuckyNumber = 3;

console.log(LuckyNumber);
//output : 3
```

**Note:** To assign value to a pre-defined binding you do not have to implictly use the special `let` keyword again. Why? We have already used it to define a binding `LuckyNumber` in the above snippet.But not essentially asked it to point at a value. So in order to make a predefined binding point at something, we just simply use the `=` operator and the expression we want the binding to grab or point at.
