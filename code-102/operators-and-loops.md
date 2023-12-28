# Operators and Loops

## Operators

> JavaScript has both *binary* and *unary operators*, and one special *ternary operator*, the conditional operator. A binary operator. A binary operator requires two operands, one before the operator and one after the operator:
> EX: operand1 operator operand2

> EX: `3 + 4` or `x * y`. This form is called an **infix binary** operator, because the operator is placed between two operands *All binary operators in JavaScript are infix.

> A **unary operator** requires a single operand, either before or after the operator:

- operator operand
- operator operand

> EX: `x++` or `++x`. The operator operand form is called a **prefix unary operator**, and the operand operator form is called a **postfix unary operator**. + + and - are the only postfix operators in JavaScript -- all other operators, like `!`, `typeof`, etc. are prefix. [^1]

# Assignment Operators

Ex: `x = f() x = f()`

Many compound assignment operators

> Name Shorthand operator Meaning

- Assignment x = f() x=f()

- Addition assignment x + = f() x = x = f()

- Subtraction assignment x -= f() x = x - f()

- Multiplication assignment x * = f() x = x* f()

- Division assignment x /= f() x = x / f()

- Remainder assignment x %= f() x = x % f()

- Exponentiation assignment x ** = f() x = x** f()

- Left shift assignment x «= f() x = x « f()

- Right shift assignment x »= f() x = x » f()

- Unsigned right shift assignment x »>= f() x = x »> f()

- Bitwise AND assignment x &= f() x = x & f()

- Bitwise XOR assignment x ^= f() x = x ^ f()

- Bitwise OR assignment x = f() x = x f()

- Logical AND assignment x &&= f() x && (x = f())

- Logical OR assignment x   = f() x   (x = f())

- Nullish coalescing assignment x ??= f() x ?? (x = f()) [^1]

- If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression. [^1]

Comparison Operators

Logical Operators

Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. The logical operators are described in the following table.

Operator Usage Description

- Logical AND (&&) - expr1 && expr2 Returns expr1 if it can be converted to false; otherwise, returns expr2. Thus, when used with Boolean values, && returns true if both operands are true; otherwise, returns false.

- Logical OR (||) - expr1 || expr2 Returns expr1 if it can be converted to true; otherwise, returns expr2. Thus, when used with Boolean values, || returns true if either operand is true; if both are false, returns false.

- Logical NOT (!) -m !expr - Returns false if its single operand that can be converted to true; otherwise, returns true.

The following code shows examples of the && (logical AND) operator.

- const a1 = true && true; // t && t returns true

- const a2 = true && false; // t && f returns false

const a3 = false && true; // f && t returns false

const a4 = false && 3 === 4; // f && f returns false

const a5 = “Cat” && “Dog”; // t && t returns Dog

const a6 = false && “Cat”; // f && t returns false

const a7 = “Cat” && false; // t && f returns false

The following code shows examples of the   (logical OR) operator.

> o1 = true   true; // t   t returns true

- const o2 = false   true; // f   t returns true

- const o3 = true   false; // t   f returns true

- const o4 = false   3 === 4; // f   f returns false

- const o5 = “Cat”   “Dog”; // t   t returns Cat

- const o6 = false   “Cat”; // f   t returns Cat

- const o7 = “Cat”   false; // t   f returns Cat

The following code shows examples of the ! (logical NOT) operator.

> const n1 = !true; // !t returns false

- const n2 = !false; // !f returns true

- const n3 = !"Cat"; // !t returns false

# Loops

For Loop

> “When there is a preset number of times that loop is going to run. That is a for loop. whether it’s one or a 1 million. It’s gonna stop when you want it to.” - Kassie

Structure:

for (initial value; condition must be true; increment/decrement){ code to execute }

let students = 13;

for (let i = 0; i < 5; i++){ console.log(‘hello to student #’, i); }

## While loop

“a ‘while loop’ is something you want to use when you don’t know how many times it’s going to take. So if you are trying to get input, from your user and you want to keep asking them until they give you an acceptable value. That is a while, loop. You don’t know how many times it’s going to take. Passwords are a ‘while’ loop”. - Kassie

Structure: while(this is true){execute this code}

EX: while (5 < 10){ Console.log('infinite looooop) }

### References

[“Expressions and operators”](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

[“Loops and iteration”](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

#### Answers

- What is an expression in JavaScript?
an expression is a valid unit of code that resolves to a value

- Why would we use a loop in our code?
Loops offer a quick and easy way to do something repeatedly

- When does a for loop stop executing?
a specified condition evaluates to false

- How many times will a while loop execute?
A while statement executes its statements as long as a specified condition evaluates to true.
