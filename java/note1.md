# Variables
***
## primitive types
- byte(0), short(0), int(0), long(0L), float(0.0f), double(0.0d), boolean(false), and char('\u0000)
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