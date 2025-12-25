# Python Syntax Basics

To start off, let's make a `program.py` file, which is a python file we'll use to run python code. Like a `-.txt` file, you can use Notepad to edit it, you don't need anything fancy.

But if you *do* want something fancy, using [IDEs](https://www.codecademy.com/article/what-is-ide) are another option, like [Visual Studio Code](https://code.visualstudio.com/), [JetBrains PyCharm](https://www.jetbrains.com/pycharm/), or even [Online Python](https://www.online-python.com/).

Once you've made the file, (if you don't know how to do this, either use the `touch` command on Linux, or right-click and `Create new file` in Windows) you now need to edit it. This depends on the editor you chose, but for now I'll assume you're using Notepad. Right click, and open with Notepad. 

Now that you're in the text editor, let's start writing some code!

Within your editor, write the following code (your first ever program!)

```python
print("Hello", "World!")
```

Woah. This is different from last time, huh? In Python, you can separate different *arguments* and print each word out with spaces between.

The alternatives are kind of scary-looking, but I promise they're not too hard.

## Concatenation

Very long word, I know. But all it means is slapping two words together with glue. That's it. Has nothing to do with cats. I think...

```python
"Hello" + " " + "World!"
```

This add the strings `"Hello"`, `" "`, and `"World!"` together, without using separate arguments, but instead one long argument that concatenated the three strings together.

There's one important thing to note. If I add numbers with strings, it doesn't work. To fix this, we'll use this thing called **typecasting**, which I'll discuss in our *Data Types* lesson.

## .join() method

All this function does is it puts spaces between the characters of a string, or the **elements** of a **list** (I will teach this to you later, I promise!)

```python
words = ["Hello", "World!"]
" ".join(words)
```

In the code example above, focus on the `join` line. We're applying the `join` method/function on the `" "` string, with `words` being used as the argument. Pretend `words` is just some pair of strings that want a `" "` between them. When we use `join()`, it adds the string you provide, in this case a `" "`, between the characters of a string, or elements of a list.

## F-strings / Formatted Strings

This lets us put **variables** inside of a string instead of adding them up, and allows us to avoid **typecasting**. 

```python
name = "Alice"
age = 30

print(f"My name is {name} and I am {age} years old.")
```

## I don't understand all these words :(

That's okay! I expect you to come back here after I've taught you those other topics. This is not a one-way thing. The only reason I've put *everything* here is that I want you to re-read and re-learn to stick it in your head, and to keep things organized. It'd be more difficult to look for, say F-strings for example, if I had put them later on in this guide than near the beginning with other string concatenation techniques.

## More on syntax

Wait wait wait. What the heck is *syntax*???

Syntax is basically just the rules of how we write Python. Just like how in English, we capitalize certain words, add punctuation, have spelling requirements, grammar, etc., so does Python! It's called **syntax**.

The basic syntax of Python is actually really easy, especially compared to other languages. Here's how it works:

- Use a `Tab` to indent code blocks inside of others, like `if` statements, `for` loops, functions, etc.
- These indents typically are made of about four spaces. If you stick to an indent size consistently, your code will work. Otherwise, you'll have errors, so pick a number and stick to it!

### Variables:
```python
x = 5
hello = "World"
cool = [1, 2, 3]
```

So these are examples of variables, where one is of *type* `int`, another is `string`/`str`, and the last is a `list`. I'll discuss these **data types** later.

Variables are basically like boxes that hold information. The `x` box holds a `5`, the `hello` box holds the word `World`, and the `cool` box...we'll talk about that later.

Lastly, there's one final thing: comments.

### Comments & Commenting

Comments are a way for your to leave little notes about your code for others, as well as to leave credits, remind yourself how a complicated piece of code works, maybe even leave some ASCII art, etc.

Comments are *very* useful, and here's how they work:

```python
print("hello") # this is a comment
# This is also a comment
# This is a comment too, and the following code won't run: print(...)

'''
this
comment
spans
multiple
lines
'''
```

And that's Python syntax!
