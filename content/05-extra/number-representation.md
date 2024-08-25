Most programming languages have multiple ways to represent numbers. In particular, they make a distinction between (integers in mathematics) and those with a decimal point (called rational numbers in mathematics). The reason is that way we encode these values in binary is different. While we don't really need to understand the full details of this encoding, we do need to understand their implications

# Integers

In mathematics, integers are simply whole numbers - ones without a fractional part, i.e. (0, 1, 2, 3, 4). They can be negative or positive, and they go on to infinity and negative infinity, though we don't typically try to count that high.

We can convert a base 10 number to base 2 pretty easily.  Let's count to 7:

| Base 10 | Base 2  |
|---------|----------|
| 0 | 0 |
| 1 | 1 |
| 2 | 10 |
| 3 | 11 |
| 4 | 100 |
| 5 | 101 |
| 6 | 110 |
| 7 | 111 |

Notice that to represent larger numbers, we need more digits? So for 0 and 1 we only needed one binary digit, for 2 and 3 we needed two binary digits, and for 4 through 7 we needed three binary digits. To represent 8, we need four. 

In fact, the maximum number we can represent in base 2 is determined by 2 to the power of the bits available, i.e. if we have 8 bits (binary digits), we can represent any number up to 255:

$$
2^8 = 256
$$

(Remember, we are also representing 0 in our 256 possible numbers).

For a computer's central processing unit to effectively do calculations, it needs to have a set amount of bits it can work with. Most modern computers use either 32 or 64 bit processors, meaning the largest positive integer they could represent are $2^{32} = 4,294,967,296$ and $2^{64} = 18,446,744,073,709,551,616$ respectively. However, that is not quite true, as we reserve one of those bits to indicate if the integer is positive and negative, and a couple of the largest possible values are reserved to represent special values like _infinity_ and _not a number_.

We don't need to know all the exact details - just that an integer in any programming language will have a maximum and minimum possible value. If we think we might need a larger (or smaller) number than that, we'll need to use a different representation.

# Rational Numbers

In mathematics, Rational numbers are those that can be expressed as a fraction of two integers $p/q$ provided $q≠0$. 

We typically represent these with a special binary encoding called _floating point_ that uses one bit to represent if the number is positive or negative, some number of bits to represent the significant digits (the fraction), and a second number of bits to represent an exponent term used to determine where the decimal point should go. The representation is similar to scientific notation:

$$
\pm[fraction] \times 10^{[exponent]}
$$

This representation allows a very large range of numbers to be represented, at the cost of precision. Mixing very large and very small numbers in algebraic operations can exacerbate this loss of precision.

There is an alternate representation, _fixed point_, which uses a similar strategy to integers, with an assumed location for the decimal point. It represents a much smaller range of numbers, but 

For most operations, we don't 