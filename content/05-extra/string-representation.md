In programming terminology, _strings_ are a sequence of characters like letters, digits, punctuation, and whitespace (spaces, tabs, and new lines). 

Each character is represented by a number of bits. One of the most popular early string encodings, ASCII used 8 bits to represent each character.  Thus, a capital **A** corresponded to the binary number **11011** (51 in base 10). With eight bits, we can represent 2⁸ possible values, or 256 characters. This is enough for both cases of the English alphabet, the Greek Alphabet, the numerals 0 to 10 and superscript and subscript versions of each, a lot of mathematical symbols, and some special symbols representing computer control signals. The standard ASCII character encodings appear in the table below:

![ASCII Encoding Table](images/asciifull.gif)

However, it was not enough to represent pictographic languages like Japanese and Chinese (there are over 50,000 kanji in the Japanese writing system). Unicode is a more modern standard that accounts for this need for additional character representation by using a variable number of bits to represent a symbol, with the first few bits indicating just how many bits are needed. 

Thankfully, we don't really need to know what the binary sequence representing a character is - the computer programs and languages we work with allow us to operate at a higher level, i.e. when we press a key on the keyboard, the character code for that key is passed to the program we are using. As long as the encoding matches what the program expects, everything works fine (but if it doesn't match, the wrong characters will be displayed, which often looks like gibberish). Moreover, Unicode's representation of English is a superset of the ASCII character encodings, so interpreting an English Unicode document as ASCII or the reverse usually works (though there may be a few odd characters).

Scratch adopts Unicode, which allows it to support a large number of languages. Now let's see how we can work with strings in Scratch.
