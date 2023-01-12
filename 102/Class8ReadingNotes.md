# Reading Notes 8

## Readings

- [Expressions and Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

- [Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

    Assignment operators assign value to its left operand based on the value of the right operand, the = is a simple assignment operator.

    Expressions that evaluate to an object of an assignment expression makes assignments based of that expressions properties; If they do not evaluate into an object then they do not assign.

        const obj = {};

        obj.x = 3;
        console.log(obj.x); // Prints 3.
        console.log(obj); // Prints { x: 3 }.

        const key = "y";
        obj[key] = 5;
        console.log(obj[key]); // Prints 5.
        console.log(obj); // Prints { x: 3, y: 5 }.


    You cannot assign properties to primitives without, you will get an error of null or undefined. The code below throws.

        const val = 0;
        val.x = 3;

        console.log(val.x); // Prints undefined.

        console.log(val); // Prints 0.


    Destructing assignment expressions make it possible to extract data from arrays or objects that mirrors the construction of array and object literals.

        const foo = ['one', 'two', 'three'];

        // without destructuring
        const one   = foo[0];
        const two   = foo[1];
        const three = foo[2];

        // with destructuring
        const [one, two, three] = foo;

    Assignments are used within a variable declaration (const, let, var) as standalone statements

    Conditional (ternary) operator is the only operator that can take 3 operands with a condition and 2 val (values)

    Unary operation is 1 operand

    Comma operator is used primarily inside a for loop to allow multiple variables through each loop.

    For, do...while, while are loops

    Break statements terminate loops

        for (let i = 0; i < a.length; i++) {
         if (a[i] === theValue){
            break;
          }
        }

    Continue statements restart while, do-while, for and label statements.

        let i = 0;
        let n = 0;
        while (i < 5) {
         i++;
         if (i === 3) {
          continue;
        }
          n += i;
          console.log(n);
        }
        //1,3,7,12

for... in statements

        for (variable in object)
          statement

for...of statements

        for (variable of object)
        statement








## Things I want to learn more about
Preeeettyyyy much all of this. Algebraically speaking, some of it makes sense like f(x) type stuff with the different types of assignments but in the terminal... and actually applying it to the code.. will be another thing. It will definitley take alot of practice to lock it down.

