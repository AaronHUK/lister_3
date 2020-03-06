# Strings and characters
In python, we call a single letter (like 'b') a **character**, and a whole word or sentence (like "Hello Lister!") a **string**.

So strings are actually just lots of characters one after another. When you have a string saved, you can even load individual characters from it! Try this:

```
displayname = input("What's your name?")
print(f"The first character of your name is {displayname[0]}")
```

The way we load individual characters from a string is with square brackets: *string*[*number*] (like displayname[0]).

Why are we asking for number 0 here?

Python counts up from 0 instead of 1, so instead of counting 1, 2, 3, 4 and so on, in python we need to count 0, 1, 2, 3, ...

This means the *first* character is [0], the *second* character is [1], and so on.

# Challenge
Can you print this: "Hello Aaron, the 3rd character is r and the 4th character is o"

<details>
  <summary>Click for hint!</summary>
  
  We can save the name to displayname like before, and then we need to print the whole name, and the 3rd and 4th characters from the name.
  
  Remember that python counts up from 0, so we'll use [2] to get the 3rd character.
</details>

<details>
  <summary>Click for answer!</summary>
  
  Try this code:
  ```python
  displayname = input("What's your name?")
  print(f"Hello {displayname}, the 3rd character is {displayname[2]} and the 4th character is {displayname[3]}")
  ```
</display>
