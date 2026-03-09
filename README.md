1. Differences Between var, let, and const
var: This creates a variable that is available throughout a whole function, or globally if placed outside a function. The computer moves it to the top of the code behind the scenes (called hoisting), and you can declare it over and over again. You can also change its value whenever you want.

let: This keeps the variable trapped inside the specific block of code (like inside { }) where you created it. The computer knows about it early on, but it isn't ready to use until the code runs. You can change its value later, but you cannot declare the exact same variable again within the same block. This helps prevent bugs caused by accidentally mixing up global variables.

const: Like let, this is also trapped inside its code block, but you must give it a value right when you create it. You cannot replace it with a new value or declare it again. If you use it for lists (arrays) or objects, the main container cannot change, but you can still update the stuff inside them.

2. The Spread Operator
The spread operator takes collections of data (like lists, text strings, or objects) and unpacks them into single, separate pieces. It is very useful when you want to make copies of data, combine different lists together, or hand off multiple values to a function.
Examples: const arr2 = [...arr1, 4];
const obj2 = {...obj1, name: "updated"};

3. Differences Between map(), filter(), and forEach()
map(): Creates a brand-new list by changing every item in the original list based on a rule you provide. The old list stays exactly the same.

filter(): Makes a new list that only includes items that pass a specific test. The original list is not changed.

forEach(): Runs a block of code for every item in your list, but it does not create a new list. It is mostly used when you just want to do an action, like printing something to the screen.

4. Arrow Functions
Arrow functions use the => symbol to write functions in a shorter, quicker way. They automatically understand the context (this) from where they were created, cannot be used to build new objects (constructors), and do not have their own built-in list of arguments.
Example: const sum = (x, y) => x + y;

5. Template Literals
Template literals are pieces of text enclosed in backticks (`) instead of regular quotes. They let you easily plug variables or math directly into the text using {...}, write text that spans across multiple lines, and make creating complex sentences much easier to read than adding strings together with plus signs.