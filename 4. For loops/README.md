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

# Challenge 1

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
  
# printing numbers in for loops

You can also use for loops to count with numbers. Try running this:

```python
num = 1
name = input("Give me your name: ")
for char in name:
  print(f"{num}: {name}")
  num = num + 1
```

<details>
  <summary>Click for hint!</summary>

  We want the first number to be 2 instead of 1, so we should start with num being 2 instead of 1.

  We also want the count to increase by 2 instead of 1, so we should add 2 in the for loop instead of 1.
</details>

<details>
  <summary>Click for answer!</summary>

  Try this code:

  ```python
num = 2
name = input("Give me your name: ")
for char in name:
  print(f"{num}: {name}")
  num = num + 2
  ```
</details>


# Challenge 2

Can you make this code count in 2s instead of 1s? e.g.

```
2: A
4: a
6: r
8: o
10: n
```

# What does this do?!

```python
displayname = input("What's your name?")
for char in displayname * 2:
  print(f"{char}")
```

# Challenge 2

Can you write a program that takes in a name and then prints this?

```
What is your name? Brian
B
rr
iii
aaaa
nnnnn
```

<details>
  <summary>Click for hint!</summary>

  We need to have a number that increases in each loop like the `num` we used above.

  Then we need to use * like the example above to print each letter more than once
 </details>

 <details>
  <summary>Click for answer!</summary>

  Try this code:
  
  ```python
name = input("What's your name?")
num = 1
for char in name:
    print(char * num)
    num = num + 1
  ```
</details>
