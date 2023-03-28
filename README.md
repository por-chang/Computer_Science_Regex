# Cpmputer Science for Regex Pal

Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ Regex is tricky to understand, but regular expressions help identifiy. As we look into a particular example that of matching an email using regular expression. This will indeed help us breaking the down components of regular expressions.

## Summary

Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

As a very visual person, something beneficial for this project was placing the regular expression in the website regex pal. From there, users can test strings. When particular strings match an expression, then they turn blue to verify a match. The user can hover over the different groups that make up the expression, and the program explains what each of the different pieces means and represents. 

To the reader, challenge yourself by viewing and attempt to create a regular expression from scratch. Even for a new user is difficult. If you are learning and new to regular expressions, it might not be very clear. However, with Regex Pal brings greater clarity to the learning process.

Start with the , which indicates a regex starting, followed by the caret ^ symbol. A caret ^ is the beginning of the line or a string.

In this particular expression, the next item, we see parentheses. Parentheses capture a group. So it is multiple tokens together, and then right after that, we have square brackets, which tell us that this is a character set and matches characters shown within this set. Inside the square brackets, there is an a-z saying that any letter between a-z is ok and may occur here, then 0-9, same thing just talking about your range of options. Any numbers between 0-9 are ok or can occur here. Immediately following the a-z0-9, there is a_which just means_and then you have an Escape character right after that, so you have got a/and a. And then there is a dash that matches the dash character saying that that is acceptable, and then we are back to our square bracket square brackets for the character set

Immediately following the square brackets, we have a +, which means that we need to match one or more than one of the tokens that we just saw. Then that is ended with parentheses to tie up that section, and then you have an @ sign, so if we are thinking of this like validating an email address, I believe it just wants to say you need to have an @ here.

Next, we have a parenthesis which means that we are now taking a look at our second capturing group, and there can be multiple tokens held within this to create this particular group. Then you have another set of square brackets to say this is a good character set, and then we have a \ and a D, which means that you can match any digit so any thing between 0 to 9. 0-9 is immediately followed by a dash see as we saw in the first group so you can have any character any letter between A-to-Z, and then we have another escape character, so we have a back/an a.

Here is what I know about escape characters. Following our escape character, the . , we have another dash - symbol, so that is just saying that is an ok option. I believe I have to look at that and then you have your square brackets just saying that is for that particular character set and a + so I can match at least one or more than one of any of these proceeding tokens that we just saw and then you have parentheses ending the capture group that we just looked at After the +), we have an escape character again . So now we are onto group 3. Hence, you start with parentheses, then you have your square brackets, and then we will determine the range again, so we have an eight Dash three, so anything between A-to-Z is ok here we have another escape character a\and a.

Then we have got a set of an end square bracket there. A quantifier occurs next, and basically, this qualifier is saying that you need to match between two and six of the preceding tokens because we have curly braces with 82, six, and then ending curly brace, and that is within parentheses. So there is our whole capture group 3, and then following that, you have the end of this regular expression which is defined with a question mark.

A question mark expresses the end of a regular expression. So you have hit the end of the regular expression.

You can tell if this works if you type in examples of email addresses below in the test string; anything that matches the above regular expression will show blue at the bottom of your page. Then it is even more incredible because you can hover over the test strings that you have created. Furthermore, it will say how your particular test string fits with this regular expression what characters or qualities it had to match your above expression.

Regex Pal is an excellent tool if you are trying to break down the different bits and pieces. Regular expressions, at first, look scary or intimidating because it is a big extended group of letters, numbers, characters, tokens, dashes, slashes +’s. It is a lot to figure out right at first. However, a significant part about this is that not only can you hover over the different pieces of this expression (and it will help you break it down), but it also has the separate parts color-coded. So a viewer can say, this is part of this, this is a part of that, and here is how they fit together. So I found this tool particularly helpful. is that not only can you hover over the different pieces of this expression and it will help you break it down, but it also has the separate parts color-coded so that you can say, ok this is part of this, this is a part of that, and here is how they fit together and so I found this tool particularly helpful

Caret ^ - the beginning of a string () captures a group $ - end of string or line [] character set a-z matches a character between a-z 0-9 matches a character between 0-9 underscore = underscore . is an escape character = - dash = dash match one or more than one of the tokens

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

Anchors include symbols like a caret and a dollar sign at the end of the string or \A letter to describe word boundaries or lack thereof. The \letter means being a or end of a string. About anchors, an example of an anchor would be a carrot a $. Anchors or a way of telling you where you are at, so basically, is it that start or the end? \A refers to the start of a string. It is probably important to note as we start to talk about anything to do with regex that regex can vary a little bit depending on which language you are looking at. Some characters are the same across multiple languages and have the same meaning, but that is not true for all of them, so it is to find good references. In the documentation I looked at, some symbols or characters or tokens had notes with them saying all engines except JavaScript, or this except for Ruby or all of these are the same depending on the language, so it is important to watch out for that. Quantifiers Examples of regular expressions quantifiers are *, +, ?, {3}, {4,7}, {5,}.

### Quantifiers

Quantifiers in regex include ?,*, +, and then items within curly braces/brackets. With quantifiers, you are basically trying to find how many times something happens or how many of certain things there are. In my research, I found that Quantifiers can also be eager reluctant possessive depending on how characters are placed together. As you hover over those different parts of the expression, it will tell you the purpose of those sets of letters or characters to help make up a particular expression. Then at the bottom of the page, they also have a nice little cheat sheet. For quantifiers, if you look at W3 schools, almost or all of the descriptions for what quantifiers start with “matches any string with” or “matches any string that.” And then in each of the examples they provide, it says more specifics, for example, matches any string with and end at the end of it or that is for the n $ example. Or it could say matches any string that is followed by a specific string, and that would be if you had a? Equals n. Basically, quantifiers tell you what to look for to match OR Operator

### Grouping Constructs

Grouping and Capturing On capturing and grouping, an easy example would be to say that you have (cat). if you are thinking about grouping and capturing and what if we use the sixth sample of the word cat with him parentheses, then a regular expression is going to look at the screw cat and convert it or instead view it as individual characters so it would be viewed as C A T

### Bracket Expressions

Bracket expressions, there is a great article I would suggest (link at the bottom of this section). In it, he breaks it down between square brackets, curly braces, and parentheses and what they each mean. Brackets tell the viewer, user, or program to look at what is in between the brackets and see if any individual characters can match. With the curly braces, they do something a little bit different their job is to say or define a specific number of things to match. So, for example, you could say I want to match this one example precisely two times. And for parentheses, these are remembered matches, so the parentheses help anytime you want to do something with a particular part of a match you can refer back to a remembered match or remembered portion of a match that would you be useful to bring up at another time

### Character Classes

Character Classes An example of character class would be a-z or A-Z - when you see this in a regular expression, it is not just talking about finding a time frame see it is saying find anything, or you can look through anything that falls in the alphabet, so anything between A-to-Z could be any one of those characters you could use this A-to-Z, or you could also think about numbers, that is a possibility with numbers as well

### The OR Operator

Alternation is actually a simple OR, which is exhibited or declared with a vertical line, so for example, if you wanted to find three different things, a cat, a dog, and a bird, you would put cat|dog|bird. this would make it so that you were requesting to look for all three of those different items are groups at the same time yeah also individually https://javascript.info/regexp-alternation

### Flags

In JavaScript, when we are talking about flags, there are only six flags that work with JavaScript and retro regular expressions; those are “I,” which is a flag that searches for casein sensitive. There is a G; this flag looks for anything without the specified request. M is multiline and makes it so that you can use a dot to match. Finally, the character U flag helps to process pairs correctly, and y is the sticky flag it looks for a particular position. https://javascript.info/regexp-introduction

### Character Escapes

Character Classes An example of character class would be a-z or A-Z - when you see this in a regular expression, it is not just talking about finding a time frame see it is saying find anything, or you can look through anything that falls in the alphabet, so anything between A-to-Z could be any one of those characters you could use this A-to-Z, or you could also think about numbers, that is a possibility with numbers as well

## Author

Por Chang

Github: https://github.com/por-chang
