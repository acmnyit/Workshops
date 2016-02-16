# Javascript Workshop : Day 2 

**Lessons** 

[TOC]

### (Do) While Loops

A do while loop is a control flow statement that executes a block of code at least once, and then repeatedly executes the block, or not, depending on a given Boolean condition at the end of the block

While Loop:

``` javascript
while (i < 10) {
	text += "The number is " + i;
    i++;
  }
```

Do While Loop:

``` javascript
var text = "";
var i = 0;
do {

    text += "The number is " + i;
    i++;
	}
while (i < 5);
```

### Recursion

Recursion is the process of defining a problem (or the solution to a problem) in terms of (a simpler version of) itself.

________________________________________________________________________________________________________________

One **example** is the calculation of factorials. The factorial of a number *n* is calculated by multiplying 1 * 2 * 3 *... *n*. The following example shows how to calculate factorials iteratively, that is, by using a **while** loop in which the result is calculated.  

``` javascript
function factorial(num)
{
    // If the number is less than 0, reject it.
    if (num < 0) {
        return -1;
    }
    // If the number is 0, its factorial is 1.
    else if (num == 0) {
        return 1;
    }
    var tmp = num;
    while (num-- > 2) {
        tmp *= num;
    }
    return tmp;
}

var result = factorial(8);
document.write(result);
```

________________________________________________________________________________________________________________

### Arrays

An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed. You have seen an example of arrays already, in the main method of the "Hello World!" application.

#### .pop()

The **pop()** method removes the last element from an array: 

``` javascript
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();
```

**Result**

`Banana,Orange,Apple`

#### .push()

The **push()** method adds a new element to an array (at the end):

``` javascript
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var x = fruits.push("Kiwi");   //  the value of x is 5		
```

**Result**

`Banana,Orange,Apple,Mango,Kiwi`

#### .join()

The **join()** method also joins all array elements into a string. It behaves just like **toString()**, but in addition you can specify the separator:

``` javascript
var fruits = ["Banana", "Orange","Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");  
```

**Result**

`Banana * Orange * Apple * Mango`

### Lists

* A **list** or sequence is an abstract data type that represents an ordered sequence of values, where the same value may occur more than once. 
* Lists are a basic example of containers, as they contain other values. If the same value occurs multiple times, each occurrence is considered a distinct item

  