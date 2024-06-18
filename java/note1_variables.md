# Variables
- stores srate of an object
- type
    - instance variable
    - class variable
    - local variable
    - parameters
- naming:
    - begins with a letter or $ or _
    - subsequent chars are letters, $, _, numbers
## primitive types
- byte(0) 8bits, short(0) 16bits, int(0) 32bits, long(0L) 64bits, float(0.0f) 32bits, double(0.0d) 64bits, boolean(false), and char('\u0000) 16bits
- compiler assigns default values to these variables but not when they are used as local variables(i.e. in methods).
## reference types
- any object (null)

# Operators
___
## conditional operators
- These operators exhibit "short-circuiting" behavior, which means that the second operand is evaluated only if needed.
- || (Logical OR)
- && (Logical AND)

## bitwise or bit shift operators
- ~ (unary bitwise complement) *// inverts a bit; 0 to 1*
- << (signed left shift) *// shifts bit pattern to the left*
- \>> (signed right shift) *// shifts bit pattern to the right*
- \>>> (unsigned right shift)
- & (bitwise AND)
- ^ (bitwise OR exclusive)
- | (bitwise OR inclusive)

## instanceof operator
- compares an object to a specified type

## other operators
- i++(postfix)
- ++i(prefix)
- ? : (ternary) *// if-then-else*

# Number and Strings
- java.lang package

## number
- wrapper classes for primitive types
- The Java compiler automatically wraps (boxes) primitives for you when necessary and unboxes them, again when necessary.
- Byte, Short, Integer, Long, Double, Float
- BigInteger, BigDecimal *//high-precision calculations*
- AtomicInteger, AtomicLong *//multithreaded apps*

### formatting
- DecimalFormat
    - java.text.DecimalFormat
    - control the display of leading and trailing zeros, prefixes and suffixes, grouping (thousands) separators, and the decimal separator.
- java.util.Formatter
- java.io.PrintStream
    - System.out *//calls the PrintStream object*
    - specifiers
        - %d%f%n

### Math
- java.lang.Math
- utility class
- methods
    - Math.cos(value)
    - Math.E(value)
    - Math.PI(value)
    - Math.abs(value)
    - Math.random()

## Character
- wrapper for primitive type char
- java.lang.Character
- immutable object
- methods
    - isLetter(c)
    - isDigit(c)
    - isWhiteSpace(c)
    - isUpperCase(c)
    - isLowerCase(c)
    - toString(c)

## String
- sequence of chars
- java.lang.String
- immutable object
- has 13 constructors
- methods
    - valueOf(n)
    - charAt(i)
    - substring(i), substring(i, i)
    - indexOf(c|s), lastIndexOf(c|s)
    - contains(s)
    - replace(c,c)
    - join(s, s...| iterable)

## autoboxing
- converting a primitive into an object
- The Java compiler applies autoboxing when a primitive value is:
  - Passed as a parameter to a method that expects an object of the corresponding wrapper class.
  - Assigned to a variable of the corresponding wrapper class.

## unboxing
- converting a wrapper object to it's corresponding primitive value 
