# Welcome to the Unofficial, Unnecessary, and completely Unwelcome COMP2300 Bit-Gauntlet!

This test of skill, willpower, and raw courage asks you to demonstrate most of
what was covered in the labs from weeks 1-6. It will either be quite challenging
or very easy depending on how well you understand bit operations, functions, and
arrays. Overall, it will probably take about an hour to get through depending on
whether or not you want to have a crack at the *super-ultra-mega-challenge*.

Because I'm bored and like chaos, there will be chocolate/some other
confectionery for the first person to get through the gauntlet. That being said
the assignment is definitely more important, so don't let me distract you if you 
haven't started.

### The rules

You will find an array in memory that represents a heavily-jumbled ascii string.
Your job is to figure out what that string says and report back. The steps for
decoding the string are provided below.

The text will be a quote from a famous book. Whoever is first to tell me which
book the quote is from wins the game! You don't have to translate the whole
quote into text; just identify what it is and where it's from.

Keep everything in assembly (except when translating the ascii into text), and
(for revision + street cred) try to use as few lines of code as possible.

### What you'll need to know

You will need to be able to:
- view data in memory, like we did in lab 1.
- perform accurate bit operations.
- iterate through *and manipulate* arrays (functions will help).

### Instructions

###### 1. Subtract 1 from all of the even-indexed bytes. Add 1 to all of the odd-indexed bytes.

###### 2. For each byte (except the first), perform an XOR operation with the previous byte.
- example:
    1. `11110000 00111100 00001111 11111111`
    2. `11110000 11001100 00001111 11111111` byte 2 is XORed with byte 1.
    3. `11110000 11001100 11000011 11111111` byte 3 is XORed with byte 2.
    4. `11110000 11001100 11000011 00111100` byte 4 is XORed with byte 3.

###### 3. For each byte, swap the first two bits with the last two bits
- examples:
    - `01000010` -> `10000001`
    - `11001100` -> `00001111`
    - etc.

###### 4. Finally, flip *all* of the bits.

###### 5. Use whatever method you like to translate enough of the ascii into text that you can identify the quote.

### Congratulations!

You've now made it to the end of the gauntlet!

BUT for *fame* and *glory* look no further than the:

### Super Ultra Mega Challenge (array *manipulation*)

For these I would recommend finding a better way of getting your ascii values out of the debugger so you can check your work. I used text editor macros.

###### 1. Remove the 2nd word (I mean an actual word, not computer .words)

###### 2. Replace the 16th word with "sad" (making the array smaller)

###### 3. Replace the 23rd word with "terrible" (making the array bigger)
