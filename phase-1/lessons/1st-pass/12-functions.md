# Functions

## Prereqs

- Data types
- Conditions
- Loops

## What are functions (Learning Objectives)

- Define a function
- Explain why you would use a function
- Inputs and Outputs (arguments)
- Why DRY code?

```
square = (x) -> x * x

cube   = (x) -> square(x) * x

area = (length, width) ->
  length * width

volume = (length, width, height) ->
  length * width * height

hello = (name) ->
  "Hello " + name

hello "Harry" #=> "Hello Harry"

hello2 = (nameArray) ->
  if nameArray.length >= 3
    "Hello #{nameArray[0]}, #{nameArray[1]} and #{nameArray[2]}"

hello2 ['Harry', 'Leo', 'Duck'] #=> "Hello Harry, Leo and Duck"
```

## With Default argument value

```
fill = (container, liquid = "coffee") ->
  "Filling the #{container} with #{liquid}..."
```

## Scope

Entering a function, is entering into another boundary

## Return

The last line of the CoffeeScript function will be returned to outer scope.

# Advanced Topics

## Mixing Object with Function

```

```

## Function with multiple return values

```
weatherReport = (location) ->
  # Make an Ajax request to fetch the weather...
  [location, 72, "Mostly Sunny"]

[city, temp, forecast] = weatherReport "Berkeley, CA"
```

## JavaScript Functions

```
#first function
var first = function () { return vegtables[0]}

first()
> "Eggplant" 

#last function

function last () { return vegtables[vegtables.length - 1] };

vegtables.first = function () {return this[0] }
vegtables.last = function () { return this[this.length - 1 ] };
vegtables.last()

var f = function() { return this[1]};

vegtables.second = f

vegtables.second()
> "Radish"


fruits.second = vegtables.second
> value

fruits.second = vegtables.second()
```

# Code Challenge

1. [First Code Challenge in CoffeeScript](https://github.com/annieccheung/wdi3-hk-code-challenge)
2. [CoffeeScript Practice](https://gist.github.com/bridgpal/c2fbca5182b4d5e53caa)