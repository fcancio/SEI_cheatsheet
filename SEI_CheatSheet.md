#CHEATSHEET

##BASH
####Navigating Your Directory
Bash | Description
:------------: | -------------
pwd | Check working directory
~ | Home directory
. | Current directory
.. | Parent directory
/ | Root directory

####Actions Within Your Directory
Bash | Description
:------------: | -------------
* | Apply to multiple items
ls | List all items in current directory
mv | Move [rename] items
cp | Copy items
touch | Create file
mkdir | Make [create] directory
add | Save changes to staging
commit | Saves and logs description of changes
push | Pushes updates to local repo to remote repo
pull | Pulls updates from remote repo into local repo
&& | Execute two commands in one line


####Options
Bash | Description
:------------: | -------------
-a | Apply to all items within directory
-f | Force apply action
-m | Provide message with action [often used with ['git commit -m]
-A | Adds new and updates items into the staging area to be committed
-r | Recurse on all subdirectories
-rm | Removes/deletes files
-rf | Removes/deltes directories

####Miscellaneous
Bash | Description
:------------: | -------------
alias | Create a shortcut command
tree | graphical representation of a directory
NaN | defines 'not a number'

####Git Actions
Bash | Description
:------------: | -------------
fork | creates a copy of a repository so you can modify without affecting the original project
git clone | clones remote repo into local repo
git add | adds new or updated files to staging area (see _'-A'_ and '_._')
git commit | commits new or updated files to github (see _'-m'_)
git push origin master | final step in pushing all modifications to local repo to github
git pull upstream master | pull latest version of remote repo to local repo

####Errors
Bash | Description
:------------: | -------------
ref | action does not have reference

##JAVASCRIPT

####Operators
Symbol | Description
:------------: | -------------
xx | adds one (1) to previous number
! | not
!! | not not 
=== | strict equality - best practice
== | performs type conversion (called coercion) if necessary
!== | strict inequality
!= | inequality
< | less than
> | greater than
<= | less than or equal
>= | greater than or equal
&& | and; always returns the first operand if it is falsey, otherwise the second operand is returned
"or operator" | or; always returns the first operand if it is truthy, otherwise the second operand is returned
? | ternary: ideal when you need to return one of two values depending upon a condition and may replace 'if/else'; ex: ```let message = score > 100 ? "You rock!" : "Keep trying!";``` **replaces** ```let message; if (score > 100) { message = "You rock!"; } else { message = "Keep trying!"; }```
/ | divide
% | modulus (division remainder)
++ | increment
- | decrement
() | group expressions


####Data Types
Term | Description
:------------: | -------------
type | a characteristic of a value affecting what kind of data it can store 
typeof | operator always returns a string describing the data type
dynamic | Dynamically-typed languages such as JavaScript, Python and Ruby allows variables to be assigned different types of data during runtime (as the program executes).
static | Statically-typed languages such as Java and C++ required a variable's type to be declared and cannot be changed:
primitive | Six primitive types in JS; data that is not an object and has no methods; are immutable
boolean | two possible values: true of false
null | represents the fact that a variable has no "real" value
undefined |
number |
BigInt |
string | represents textual data with zero or more characters wrapped by single or double quotation marks such as "John" or 'Jane'. A pair of quotes with nothing between them is still a string - an empty string.
symbol |
RegExp | uses '//' to define expression not to be included in code
Data | 
complex/reference | 
object |
array | store multiple items in a variable
function | A function is a reusable block of code designed to perform a single purpose. It optionally takes in data as input and returns a single piece of data (including complex data such as objects, functions, etc.).


####Variable Identifiers
Term | Syntax | Description
:------------: | :-------------: | ------------
scope | | The difference between var and let/const is what we call scope. Scope revolves around the accessibility of variables & functions at a given point in the code.  var has function scope (also known as local scope) and let/const have more limited block scope, which in computer programming, is considered a better practice because it reduces the chance of accidentally changing a variable's value.
var |
let |
const | ```const person = {name: 'Fred'};``` | variable cannot be reassigned to
 | ```person.age = 25;```  | no error  
 | ```person = {name: 'Barney'}```  | Uncaught TypeError: Assignment to constant


####Browser Shortcuts
Term | Syntax | Description
:------------: | :-------------: | ------------
option + command + J | | opens console
option + command + I | | opens console

##Arrays

####Top 10 Array Methods
Term | Syntax | Description
:------------: | :-------------: | ------------
array | let array1 = [ 'x', 'y', 'z']; | stores multiple items in a variable
forEach | array1.forEach(function(element)) { | defines function for each element within array

####Common Array Phrases
Term | Syntax | Description
:------------: | :-------------: | ------------
 | const element = [x, y, z] |
 
##Functions
####Terms to know
Term | Syntax | Description
:------------: | ------------- | ------------
call, execute, invoke or "run a function" | |
parameter | |
argument | |
scope | |
scope chain | | _(see 'reference error')_
global scope | | at the top of the scope chain and its properties are available to every function we write; accessible from anywhere


function scope | |
block scope | |
lexical scope | |
module scope | |

####Types of Functions
Term | Syntax | Description
:------------: | ------------- | ------------
declaration |```function fnDeclaration() { console.log("I'm coming from a function declaration"); }``` |
expressions | ```const fnExpression = function() { console.log("I'm coming from a function expression"); };``` |
arrow | ```const add = (a, b) => a + b;``` | more concise; implicit return of a single expression; a single rule for binding the ```this``` keyword

 
####Best Practices
Practice | Why
:------------: | -------------
 DRY | 'Don't repeat yourself'; makes maintaining code easier as well as streamlines program execution; tackle complexity; allows you to reuse code; allows you to debug your application
 stub up | create a skeleton for the code
 indent | indent appropriately for better readability of your code
shit + option + down arrow | on current line of code, copies that code to the following line
string interpolation | use backticks (`) to wrap your expression and type '$' in front of {value}
rest parameters (...) | 
default parameters | use 'or' symbol to provide default parameter if variable parameter is undefined
 