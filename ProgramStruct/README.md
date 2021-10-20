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
