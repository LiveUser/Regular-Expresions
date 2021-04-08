# Regular Expressions

Some of the basics I could get from a YouTube Video for me and all of you to use as reference. May have errors, I transcribed almost everything. Watching the video would also come in handy.

Hecho en 🇵🇷 por Radamés J. Valentín Reyes

## Global Selection

Find all of the occurrences of the string

~~~RegEx
/findMe/g
~~~

## Case insensitive Global

Does not care about upper or lower case letters

~~~RegEx
/findMe/gi
~~~

## Find at least one

Find at least one of the characters || String

~~~RegEx
/findMe+/g
~~~

## Optional selection

Make the character before the ? optional

~~~RegEx
/findMe?/g
~~~

## Star indicator

matches as many characters before * as possible

~~~RegEx
/findMe*/g
~~~

## Period

Matches every word that contains the specified string entirely. The period goes before what you want to match.

~~~RegEx
/.findMe/g
~~~

## Have a period as string

Search for the period rather than using it as the the operator before

Example: Looks up .findMe

~~~RegEx
/\.findMe/g
~~~

## Select/Find words

Selects all words

~~~RegEx
/\w/g
~~~

## Select spaces

Selects all spaces (waste spaces)

~~~RegEx
/\w/g
~~~

## Select words by size

Put the word length inside curly braces

~~~RegEx
/\w{4}/g
~~~

If it can have multiple sizes, separate the sized by a coma.

~~~RegEx
/\w{4,5}/g
~~~

## Character Set

Matches any character inside the set. Characters are placed inside [ ].

Example: the character set includes the letters f, i, n, d

~~~RegEx
/[find]en/g
~~~

## Character range

A range of characters rather than a specific character by placing the range between brackets and separating it with a -

~~~RegEx
/[a-z]/g
~~~

## Making groups and using pipes

Groups go between parenthesis.

| (pipes) function as the OR operator in programming

~~~RegEx
/(t|T){2,3}he/g
~~~

## Matching the beginning of the line

Use the ^ symbol for this operation

~~~RegEx
/^T/g
~~~

## Matching the end of the statement

Use the $ symbol after the letter

~~~RegEx
/m$/g
~~~

## Positive Look Behind

~~~RegEx
/(?<=[find]me)/g
~~~

## Negative Look Behind

~~~RegEx
/(?<![find]me)/g
~~~

## Select everything that does not have after the text you wrote

~~~RegEx
/.(?!at)/g
~~~

## Specify the amount of digits

\d stands for digits

~~~RegEx
/\d{10}/g
~~~

## Name the data

Just to make sure that you know what you are reading

~~~RegEx
/?<areacode>/g
~~~



# Where to practice the skills

https://regexr.com/

# References:

- https://www.youtube.com/watch?v=rhzKDrUiJVk