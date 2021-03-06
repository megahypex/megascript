<h1>Arrays</h1>

Arrays are storage structures which store multiple values within them, which can be accessed by an index.<br>
Every value has a unique index which shows its position in the array.<br>
MegaScript is `0` indexed, which means that all indexes start from `0` and proceed. 
<br><br>
An array can be defined using pairs of square brackets `[]` with initial values in the middle, separated by commas.
```
var array = ["Apple", "Orange", "Banana"]
```
And they can be indexed like so:
```
var array = ["Apple", "Orange", "Banana"]
var first = array[0]        // `first` gets set to "Apple"
var second = array[1]       // `second` gets set to "Orange"
```
Index `0` represents the first element, `1` second, and so on.<br>
Arrays are normal values and can be passed around, as arguments and variables. 
Values in arrays can be modified using their index<br>
```
var array = ["abc"]
array[0] = "xyz"

var value = array[0]      // = "xyz"
```

<h4>Array ranges</h4>

Array ranging is a feature which makes it easier to fill arrays with a predictable sequence of numbers<br>
You can pass the start value and end value, and it will automatically get filled in with the corresponding number range.
```
var array = [0..5]      // = [0, 1, 2, 3, 4, 5]
```
An increment can also be provided, which skips the numbers accordingly, by default the increment is `1`
```
var array1 = [5..0..-1]       // = [5, 4, 3, 2, 1, 0]
var array2 = [0..10..2]       // = [0, 2, 4, 6, 8, 10]
```

<h2>Bound Methods</h2>

Following are the methods bound to every array object.

1. `array.insert(...)` : This method inserts all the arguments passed to it as elements in order.
<br>Example:
```
var array = []
array.insert(10, 20, "a")
```

[previous](/docs/functions.md) | [next](/docs/tables.md) | [index](/docs/documentation.md)
