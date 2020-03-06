# Input
Sometimes we want to be able to tell python what to print. We can ask for input from the user to do this. Try this:

```
displayname = input("What's your name?")
print(f"Hello {displayname}!")
```

Try running the first line by itself:

```
displayname = input("What's your name?")
```

See the difference in what's shown on the screen. What's happening here?

This line is just **saving** the name you give it to the **variable** displayname - but doesn't ever use the name we've given it!

The second line:

```
print(f"Hello {displayname}!")
```

**Loads** the name we saved into displayname and puts it into the text!

What happens if we try to load displayname with the second line before we've saved it with the first line?

# Challenge 1

Can you print "Nice to see you, Aaron, how are you?" on the next line?
<details>
  <summary>Click for hint!</summary>
  
  You don't need to save the name twice, you only need to print twice!
  
  What happens if we add another print statement on the next line that also uses **displayname**?
</details>

<details>
  <summary>Click for answer!</summary>
  
  Try this code:
  ```python
  displayname = input("What's your name?")
  print(f"Hello {displayname}!")
  print(f"Nice to see you, {displayname}, how are you?")
  ```
</details>

# Challenge 2

Can you ask for two names, and then print "Aaron and Tim are programmers"?
<details>
  <summary>Click for hint!</summary>
  
  It's easiest to have 2 separate input lines, saving the names to displayname1 and displayname2.
</details>

<details>
  <summary>Click for answer!</summary>
  
  Try this code:
  ```python
  displayname1 = input("What's the first name?")
  displayname2 = input("What's the second name?")
  print(f"{displayname1} and {displayname2} are programmers")
  ```
</details>
