# For loops

If we're looking at the individual characters in a string, we often want to go over *every* character without having to specify [0], [1], [2], ...

We can do this with a for loop!

```python
displayname = input("What's your name?")

for char in displayname:
  print(f"! {char} !")
```

Note that the print line there has 2 spaces at the start - the text is **indented** and this **indent** controls which lines run in the for loop.

Here's a more complex demonstration of how the indenting works:

```python
displayname = input("What's your name?")

print("I know your name now, let me spell it...")

for char in displayname:
  print("Let me see, the next letter was:")
  print(f"{char}!")

print("I'm done spelling your name now :)")
```

Here we indented **2** lines, and *both* lines were run *for every* character in the name. We can run as much code in the for loop as we want, as long as we indent them!

The last line was not indented, and so was not in the for loop - it only printed once.

# Challenge

Can you take someone's name, and then print it out like this?
```
What's your name?Brian
Brian!
B B 
B B
r r
r r
i i
i i
a a
a a
n n
n n
Brian!
```

<details>
  <summary>Click for hint!</summary>
  
  We want to print the name once before the for loop, and once afterwards.
  
  In the for loop itself, we want to print 2 lines for each character, so we should have 2 print statements.
</details>

<details>
  <summary>Click for answer!</summary>
  
  Try this code:
  
  ```python
  displayname = input("What's your name?")
  print(f"{displayname}!")
  for char in displayname:
    print(f"{char} {char}")
    print(f"{char} {char}")
  print(f"{displayname}!")
  ```
</details>
  
# What does this do?!

```python
displayname = input("What's your name?")
for char in displayname * 2:
  print(f"{char}")
```

  
