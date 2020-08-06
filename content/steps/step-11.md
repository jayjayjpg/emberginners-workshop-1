---
title: Step 11 - Git Clone
order: 11
---

## Exercise 2a: Cloning a git repo

To clone a git repo you can run the following:

```bash
git clone https://github.com/simplabs/emberginners-workshop-app.git
```

this will create a folder called `emberginners-workshop-app` that you can `cd` into.

Something to note when you're cloning a repo that uses npm, you need to install the repos depenedencies before you can do anything

```bash
cd emberginners-workshop-app

npm install
```

## Exercise 2b: Run JavaScript from a file

- Open your text editor
- Open the new folder that was created when we used `git clone`
- start the server using `npm start`
- visit [http://localhost:4200/demos/demo-2b.html](http://localhost:4200/demos/demo-2b.html)
  - you should see "hello there" but nothing should happen
- Open the file `/public/demo/demo-2b.html` in your text editor
- Investigate the `<script type="text/javascript"></script>` section in your editor
- Fill in a snippet of JavaScript code from the previous exercise (1a) into the snippet below the `// comment`
- Reload the page in the browser. What do you see?
- Trouble with the exercise? Open `/public/demo/demo-2b-solution.html` in your editor and browser

## What are variables?

Variables in JavaScript provide a way to **store** and to **retrieve** words, numbers and other more complex things in your program.
A variable acts as a container for these so-called _values_. You can _declare_ a variable and fill it in with a value by using a dedicated keyword and the _assign_ operator `=`.

In the scope of this workshop we will learn about one particular variable keyword called `let`. If you continue to learn more about JavaScript after this workshop, you might encounter other variable keywords as well, but for now, we can do everything we want to achieve in this course by focussing on `let` only.

If you, for example, wanted to create a variable that stores your favorite color, can write the following:

```js
let color = 'purple';
```

This line does 3 things:

- It creates a new variable, a container for any word or number you want to store
- It fills in the variable `color` with the word `purple`
- It allows you to retrieve the word `purple` any time again in your code by reading from the variable `color`

You can choose almost any word that comes to your mind, when naming a variable. It's also possible to include numbers in your variable name.

After a variable has been declared, you can read its value by using its name further down your program:


```js
let color = 'purple';

// ...other code

console.log(color);
// => prints "purple" to your console
```

Also, after a variable has been declared for the first time, you can update its value anytime further down in your code as follows:

```js
let color = 'purple';

// ...other code

color = 'blue';
```

When **updating** an **already declared** variable, you **must not** use the variable keyword. The variable keyword is only used when you declare a new variable for the first time.

Besides that, we also see that each code instruction - a so-called _statement_ - ends with a semi-colon `;`. It acts as like a colon after a phrase indicating to the browser that a full code instruction ends right there.

Note: In the examples above we're assigning a word, or a so-called _string_, to our variable `color`. A string describes a number of characters, either letters, numbers or special characters, which are _stringed_ together. A string always needs to be written in quotation marks - you are free to choose either single quotes `'` or double quotes `"`.

## Exercise 2c: Read and write to variables

- Open the file `/public/demo/demo-2c.html` in your text editor
- visit [http://localhost:4200/demos/demo-2c.html](http://localhost:4200/demos/demo-2c.html)
- Investigate the current `alert()` statement in your editor. What do you see?
- Open your browser console (as described in Exercise 1a). What does the error message tell you about what is happening on the website? Try clicking the link that is provided with the error message. What do you see?
- Find out how to make your page alert the phrase `I learn all day` without changing the line with the `alert` statement
- Make your program alert `I learn all day` first and then alert `I code all day` second by using only one variable in your program
