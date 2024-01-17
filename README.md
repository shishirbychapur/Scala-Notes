# Scala-Notes

## Syntax

### Defining a type in scala:

```scala
var a: Int = 10
```

### Defining a function in scala: (Have to specify types of parameters of a function, return type is optional)

```scala
def add(x: Int, y: Int): Int = x + y
```

### If-Else Statements:

```scala
val m = if (a > b) a else b
```

### Try-Catch Statements:

```scala
try {
    …
} catch {
    case x: exception => 0
}
finally {
    …
}
```

### Print variable values:

```scala
println(s”the value of x is $x”)
```
## Data Structures

### Tuples: (Doesn’t necessarily have to be limited to a pair and elements don’t have to be the same data type)

```scala
tup._1     // Access the first element of the tuple
tup._2   // Access the second element of the tuple
```

### Arrays are mutable, Lists are immutable

### Empty Lists are represented as `Nil`

#### Adding to head of the list: [Right associative]

```scala
Nil.::(1)         // Output is List(1)
Nil.::(1)::(2) // Output is List(2, 1)
1 :: 2 :: 3 :: Nil     // List(1, 2, 3)
```

#### Concatenate two lists:

```scala
List1 ::: List2
```

#### Iterating through a map:

```scala
for((step, instruction) <- maps) { }
```
## Object Oriented Programming

### No explicit constructor for classes (Class takes in a parameter if required)

### Class parameters are not fields inside the class. To make them accessible, add the “val” keyword

### Scala object is a singleton instance (no static/class level members)

### Scala companions can access each other’s private members
