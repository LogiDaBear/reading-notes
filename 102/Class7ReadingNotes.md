# Reading Notes 7

## Readings

- [Control Flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)

- [Functions](https://www.w3schools.com/js/js_functions.asp)

- [Operators](https://www.w3schools.com/js/js_operators.asp)

### Notes

    Conditionals and loops can change the control flow of how code is processed. Reading from start to finish

    functions can contain multiple parameters by seperating each one with a comma

    Function is a block of code designed to perform a particular task and when executed "something" has called it/invoked it. Like summoning a demon.

    Chaining or nesting an assignment expression is discouraged but sometimes is in code so here is an example of said discouragement... 
    let x;
    const y = (x = f()); // Or equivalently: const y = x = f();
    console.log(y); // Logs the return value of the assignment x = f().

    console.log(x = f()); // Logs the return value directly.

    // An assignment expression can be nested in any place
    // where expressions are generally allowed,
    // such as array literals' elements or as function calls' arguments.
    console.log([ 0, x = f(), 0 ]);
    console.log(f(0, x = f(), 0));...

    


### operators

    +	Addition
    -	Subtraction
    *	Multiplication
    **	Exponentiation (ES2016)
    /	Division
    %	Modulus (Division Remainder)
    ++	Increment
    --	Decrement 

    =	Ex: x = y    Same as: x = y
    +=	    x += y	          x = x + y
    -=	    x -= y	          x = x - y
    *=	    x *= y	          x = x * y
    /=	    x /= y	          x = x / y
    %=	    x %= y	          x = x % y
    **=	    x **= y	          x = x ** y

    ==	equal to
    ===	equal value and equal type
    !=	not equal
    !==	not equal value or not equal type
    >	greater than
    <	less than
    >=	greater than or equal to
    <=	less than or equal to
    ?	ternary operator
    &&	logical and
    ||	logical or
    !	logical not

    typeof:	Returns the type of a variable

    instanceof:	Returns true if an object is an instance of an object type



## Things I want to learn more aboot
variables answers converted to all caps (.toUpperCase) or lowercase (.toLowerCase) based on your variable typing. DONT do both such as 'Yellow': Figuring out how to incorporate both.

What the order in pemdas is for '2'+ 2 * '2' i.e- using quotes in java

Conditionals that make the loops and functions determine wrong and right answers in order to get out of said loops/functions.

