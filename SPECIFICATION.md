# Basic Syntax

This serves as a brief guide and quick start to the basic syntax behind utilising aurora

## What is this?
Aurora is a configuration language project designed to permit maximum customisability to the program that utilises it along with being simple to understand for the end user.

 **It is not a programming language and should not be treated like one**.

## Comments

Aurora supports both single-line and multi-line comments. Users of the language should utilise them to explain their configuration choices.

**Single-Line**
```
// This is a comment
<other code>
```

**Multi-line**
```
/* 
    This is a multi line comment
    It comments out whole blocks between /* and */
*/
```

## Types

Aurora features a very basic type system featuring primitive types and some more complex collections.

**Primitive Types**

| Type | Description                            | Representation                                                |
|------|----------------------------------------|---------------------------------------------------------------|
| char | A single character                     | Wrapping a character in single quotes ``''``                  |
| num  | Any decimal number                     | Writing the decimal number in plain text e.g ``5`` or ``6.7`` |
| bool | A Boolean value, ``true`` or ``false`` | Writing the keywords ``true`` or ``false``                    |

**Collections**

| Type   | Description                                     | Representation                                                               |
|--------|-------------------------------------------------|------------------------------------------------------------------------------|
| list   | An unordered collection of one or more elements | Wrapping comma seperated elements in ``[]``                                  |
| string | A ``list`` of characters (``char``)             | Wrapping multiple characters in ``""``                                       |
| map    | A collection of key, value pairs                | Constructed with ``{}`` around ``key: value`` pairs that are comma seperated |

## Variables

In Aurora variables can be used to hold any value/type, they are immutable and cannot be redefined/modified.

**Defining a variable**

Variables are defined through use of the equals sign with the name of the variable on the left hand side, and the value on the right hand side on the same line e.g:

```
// Valid variables
foo = "bar"
baz = 5.0

// Invalid, Value must be on same line
bah = 
5

// Invalid, Variables are immutable and we cannot
// redefine them
foo = "beh"
```