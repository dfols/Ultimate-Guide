# Ultimate Study Guide

## Table of Contents

### [Introduction](#introduction)

- [How To Use This Guide](#how-to-use-this-guide)
- [Installation](#installation)

### [Command Line Interface (CLI)](#command-line-interface-cli)

- [What is CLI?](#what-is-cli)
- [Why Should I Learn Command Line?](#why-should-i-learn-command-line)
- [Shell vs. Terminal](#shell-vs-terminal)
- [Common Commands](#common-commands)
- [Example Workflow](#example-workflow)

### [Git](#git)

- [What is Git?](#what-is-git)
- [Why Should I Learn Git?](#why-should-i-learn-git)
- [Git vs. GitHub](#git-vs-github)
- [Basic Git Commands](#basic-git-commands)
- [Working with Branches](#working-with-branches)
- [Understanding Origin](#understanding-origin)

### [HTML](#html)

- [What is HTML?](#what-is-html)
- [Why Should I Learn HTML?](#why-should-i-learn-html)
- [Document Structure](#document-structure)
- [Inline vs Block Elements](#inline-vs-block-elements)
- [Semantic HTML](#semantic-html)
- [Headings and Paragraphs](#headings-and-paragraphs)
- [Lists](#lists)
- [Images](#images)
- [Links](#links)
- [Forms and Inputs](#forms-and-inputs)
- [Labels](#labels)
- [Tables](#tables)
- [Block and Inline Elements](#block-and-inline-elements)

### [CSS](#css)

- [What is CSS?](#what-is-css)
- [Why Should I Learn CSS?](#why-should-i-learn-css)
- [How to Apply Styles](#how-to-apply-styles)
- [Selectors](#selectors)
- [Common CSS Properties](#common-css-properties)
- [Box Model](#box-model)
- [Flexbox](#flexbox)
- [Grid](#grid)
- [Media Queries](#media-queries)

### [JavaScript](#javascript)

- [What is JavaScript?](#what-is-javascript)
- [Why Should I Learn JavaScript?](#why-should-i-learn-javascript)
- [Types of Values](#types-of-values)
- [Type Conversion](#type-conversion)
- [Operators](#operators)
- [Modifying Variables in Place](#modifying-variables-in-place)
- [Comparisons](#comparisons)
- [Conditionals](#conditionals)
- [Loops](#loops)
- [Functions](#functions)
- [Arrays](#arrays)
- [Objects](#objects)
- [Constructor and "new" Operator](#constructor-and-new-operator)
- [This](#this)
- [Arrow Functions](#arrow-functions)

## Introduction

Welcome to the Ultimate Guide! This guide covers the basics of Command Line
Interface (CLI), HTML, CSS, JavaScript, and Git, providing you with the
foundational knowledge needed to start building websites and managing code
repositories.

### How To Use This Guide

This guide is structured into sections, each focusing on a different aspect of
web development. It is recommended that you follow the guide in order,
especially if you are new to these concepts. However, if you are already
familiar with some topics, feel free to jump to the sections that interest you
the most. Each section will have explanations accompanied by code examples and
best practices to help you understand the concepts better.

### Installation

Before we start, let's make sure you have all the necessary software installed:

1. **Text Editor**: Download and install a text editor of your choice. Visual
   Studio Code is highly recommended for its extensive features and community
   support.

2. **Git**: Git is essential for version control. You can download it from the
   [official website](https://git-scm.com/downloads). Follow the instructions
   for your operating system.

3. **Node.js (Optional for JavaScript)**: If you plan on diving deep into
   JavaScript, it’s good to have Node.js installed. This allows you to run
   JavaScript code outside of the browser. You can download it from the
   [official website](https://nodejs.org/en/download/).

4. **Web Browser**: Make sure you have a modern web browser installed. This will
   be necessary for viewing your HTML and CSS in action.

Once you have these tools installed, you're ready to dive into the exciting
world of web development!

## Command Line Interface (CLI)

### What is CLI?

The Command Line Interface (CLI) is a user interface that allows you to interact
with your computer using text-based commands.

### Why Should I Learn Command Line?

- Direct interaction with the operating system.
- Automating tasks using scripts.
- Essential for software development and system administration.

### Shell vs. Terminal

- **Shell**: A shell is a program that processes commands and returns output.
  It's an interface that allows users to interact with the operating system by
  entering commands. Shells can be interactive or used to execute scripts.

- **Terminal**: A terminal, also known as a terminal emulator, is a program that
  provides the text-based interface to the shell. The terminal emulates a
  console, allowing users to type in shell commands. It sends the commands to
  the shell for processing and then displays the output. The terminal itself
  doesn't handle command processing; it's just the interface to the shell.

### Common Commands

- `cd`: Change Directory. Use this to navigate through directories.

```sh
cd Documents
```

- `ls`: List files and directories. Use this to view the contents of a
  directory.

```sh
ls
```

- `pwd`: Print Working Directory - shows the current directory path.

```sh
pwd
```

- `mkdir`: Make a directory. Use this to create a new directory.

```sh
mkdir my_directory
```

- `rmdir`: Remove an empty directory. Use this to delete an empty directory.

```sh
rmdir my_empty_directory
```

- `rm`: Remove files or directories. Use this to delete files or directories.

```sh
rm file.txt
```

- `cp`: Copy files or directories. Use this to create a copy of files or
  directories.

```sh
cp source.txt destination.txt
```

- `mv`: Move files or directories. Use this to move files or directories to a
  new location.

```sh
mv file.txt my_directory/
```

- `echo`: Display a line of text. Useful for printing messages.

```sh
echo "Hello, World!"
```

- `cat`: Display the content of files. Use this to read the contents of a file.

```sh
cat file.txt
```

- `grep`: Search for a specific pattern within a file. Useful for searching
  within files.

```sh
grep "hello" file.txt
```

- `sudo`: Execute a command with superuser permissions.

```sh
sudo apt-get update
```

- `man`: Display the user manual for a command. Useful to get more information
  about a command.

```sh
man ls
```

### Understanding `.` and `..`

`.` represents the current directory. `..` represents the parent directory.

These can be used in combination with the `cd` command for navigating
directories. For example, `cd ..` moves you up one directory, and `cd .` does
nothing as it keeps you in the current directory.

### Example Workflow

Here's an example workflow combining the commands above:

```sh
mkdir my_project              # Create a new directory named "my_project"
cd my_project                 # Change directory to the newly created directory
echo "Hello, World!" > hello.txt  # Create a new file named "hello.txt" and write "Hello, World!" into it
cd ..                         # Go back to the parent directory
mkdir another_directory       # Create another directory named "another_directory"
mv my_project/hello.txt another_directory/  # Move the hello.txt file from my_project to another_directory
```

This example creates a new directory, changes the current directory to the one
just created, creates a file within it, then goes back to the parent directory
and moves the file into another directory.

## Git

### What is Git?

Git is a distributed version control system for tracking changes in source code.
It allows multiple developers to work on the same codebase without overwriting
each other's changes. Git stores code history, so you can revert to previous
versions if needed.

### Why Should I Learn Git?

- **Collaborate on code with others**: Git enables multiple developers to work
  on the same project simultaneously.
- **Keep a history of changes**: You can view the history, find out who made
  which changes, and revert to a previous state if necessary.
- **Merge code and resolve conflicts**: Combine code from different branches and
  resolve conflicts when they arise.

### Git vs. GitHub

**Git**:

- It is a version control system.
- You can use Git locally on your computer.
- Git helps you manage the history and collaboration of your code.

**GitHub**:

- GitHub is a web-based platform.
- You can host your Git repositories online on GitHub.
- It provides additional features like Pull Requests, Issues, and a web-based
  interface for repository management.

While Git is essential for version control, GitHub adds an extra layer of
functionality, particularly for collaboration across teams and the open-source
community.

### Basic Git Commands with Examples

- **`git init`**: Initialize a new Git repository. This command creates a new
  `.git` directory in your project to track the repository's metadata and object
  database.

```sh
git init
```

- **`git add`**: Stage changes for commit. This tells Git that you want to
  include the updates to a particular file in the next commit.

```sh
git add filename
```

To add everything in the directory:

```sh
git add .
```

- **`git commit`**: Commit staged changes. This captures a snapshot of the
  project’s currently staged changes.

```sh
git commit -m "Your commit message here"
```

- **`git push`**: Push commits to a remote repository. This sends the committed
  changes to a remote repository like GitHub.

```sh
git push origin main
```

Here, `origin` is the default name Git gives to the server you cloned from, and
`main` is the branch you are pushing to.

- **`git pull`**: Fetch and integrate changes from a remote repository. This
  command is used to fetch changes from the remote repo and merge it into the
  current branch.

```sh
git pull origin main
```

- **`git branch`**: List, create, or delete branches. This command allows you to
  work with branches.

To list branches:

```sh
git branch
```

To create a new branch:

```sh
git branch new-branch
```

To delete a branch:

```sh
git branch -d branch-name
```

To switch to a different branch:

```sh
git checkout branch-name
```

### Working with Branches

Branches are used for developing features isolated from each other. The `main`
branch is the default branch when you create a repository. Use other branches
for development and merge them back to the `main` branch upon completion.

Example:

```sh
git checkout -b feature-branch   # Create and switch to a new branch named "feature-branch"

touch file  # Make changes
git add . # Stage
git commit -m "message" # Commit

git checkout main                # Switch back to the main branch
git merge feature-branch         # Merge the feature branch into the main branch
```

This example demonstrates how to create a new branch, switch to it, make
changes, and then merge those changes back into the main branch.

### Understanding Origin

In Git, `origin` is the default name given to the remote repository where you
want to publish your commits. It's essentially a shorthand name for the remote
repository's URL. For example, when you run the command `git push origin main`,
you're telling Git to push your changes to the main branch on the remote
repository associated with `origin`.

## HTML

### What is HTML?

HTML (Hypertext Markup Language) is the standard markup language for documents
designed to be displayed in a web browser. It helps structure the content and
present it on the web.

### Why Should I Learn HTML?

HTML is the backbone of web pages. Learning HTML is essential for anyone
interested in web development or design, as it's the basic building block for
creating websites.

### Document Structure

An HTML document has a specific structure that includes `<!DOCTYPE html>`,
`<html>`, `<head>`, and `<body>` elements.

- **`<!DOCTYPE html>`**: Declares the document type and version of HTML.
- **`<html>`**: The root element that contains all the content of the document.
- **`<head>`**: Contains meta-information about the document such as its title.
- **`<body>`**: Contains the content that is visible to users.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Web Page</title>
  </head>
  <body>
    <!-- Visible content goes here -->
  </body>
</html>
```

### Inline vs Block Elements

**Inline Elements**: Do not start on a new line and only take up as much width
as necessary. Example: `<span>`, `<a>`.

```html
This is <span>inline</span> element.
```

**Block Elements**: Start on a new line and take up the full width available.
Example: `<div>`, `<h1>`, `<p>`.

```html
<div>This is a block element.</div>
```

### Semantic HTML

Semantic HTML elements are those that clearly describe their meaning in a human
and machine-readable way. Examples include `<header>`, `<footer>`, `<article>`,
and `<section>`. Using semantic tags helps improve the structure and
accessibility of web content.

```html
<article>
  <header>
    <h1>Article Title</h1>
  </header>
  <section>
    <p>Content of the article...</p>
  </section>
  <footer>
    <p>Article footer.</p>
  </footer>
</article>
```

### Headings and Paragraphs

Headings and paragraphs are fundamental building blocks of any web page.
Headings are used to define the structure and layout of your content. Paragraphs
are used for regular text.

HTML headings are defined with the `<h1>` to `<h6>` tags, with `<h1>` being the
largest and `<h6>` the smallest.

```html
<h1>This is a heading level 1</h1>
<h2>This is a heading level 2</h2>
<h3>This is a heading level 3</h3>
<p>This is a paragraph.</p>
```

### Lists

There are two types of lists in HTML: unordered lists and ordered lists. An
unordered list is a collection of items that do not have a numerical order. This
is created using the `<ul>` element. An ordered list is a collection of items
that are numbered in order. This is created using the `<ol>` element.

```html
<!-- Unordered list -->
<ul>
  <li>Apple</li>
  <li>Banana</li>
  <li>Cherry</li>
</ul>

<!-- Ordered list -->
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

#### Images

The `<img>` tag is used to embed images in a document. The `src` attribute
contains the image URL and is mandatory. The `alt` attribute provides
alternative text for the image if it cannot be displayed.

```html
<img src="url-of-your-image.jpg" alt="Description of the image" />
```

### Links

Links are used to navigate between pages on the internet. The `<a>` tag is used
to create hyperlinks.

Basic link example:

```html
<a href="path-to-file.html">This is a link</a>
```

Open link in a new tab:

```html
<a href="https://example.com" target="_blank">Open in new tab</a>
```

### Forms and Inputs

Forms are essential for collecting data from the user. The `<form>` element is
used to create a form, and within this, various input elements and buttons can
be placed.

**Text Input**: For general text input.

```html
<input type="text" name="username" placeholder="Enter your username" />
```

**Password Input**: For password entry fields. Characters are obscured.

```html
<input type="password" name="password" placeholder="Enter your password" />
```

**Radio Buttons**: Let the user select one option from a set.

```html
<input type="radio" name="gender" value="male" /> Male
<input type="radio" name="gender" value="female" /> Female
```

**Checkboxes**: Allow the user to select multiple options.

```html
<input type="checkbox" name="option1" value="Option 1" /> Option 1
<input type="checkbox" name="option2" value="Option 2" /> Option 2
```

**Submit Button**: Used to submit a form.

```html
<input type="submit" value="Submit" />
```

**Email Input**: For email addresses.

```html
<input type="email" name="email" placeholder="Enter your email" />
```

**Number Input**: For numeric input.

```html
<input type="number" name="quantity" min="1" max="10" />
```

**Date Input**: For date input.

```html
<input type="date" name="birthday" />
```

### Labels

The `<label>` element is an essential part of forms. It is used to add text next
to an input element, improving usability and accessibility. The `for` attribute
in the `<label>` should have the same value as the `id` attribute of the input
it's associated with. This allows users to click the label to focus/select the
input element.

Here's how you can use the `<label>` element in conjunction with different input
types:

```html
<!-- Text input with label -->
<label for="username">Username:</label>
<input
  type="text"
  id="username"
  name="username"
  placeholder="Enter your username"
/>

<!-- Password input with label -->
<label for="password">Password:</label>
<input
  type="password"
  id="password"
  name="password"
  placeholder="Enter your password"
/>

<!-- Radio buttons with labels -->
<label for="male">Male</label>
<input type="radio" id="male" name="gender" value="male" />
<label for="female">Female</label>
<input type="radio" id="female" name="gender" value="female" />

<!-- Checkbox with label -->
<label for="option1">Option 1</label>
<input type="checkbox" id="option1" name="option1" value="Option 1" />

<!-- Number input with label -->
<label for="quantity">Quantity (between 1 and 10):</label>
<input type="number" id="quantity" name="quantity" min="1" max="10" />
```

Using labels not only makes the form more user-friendly but also makes it more
accessible to screen readers, improving the overall accessibility of your
webpage.

### Tables

Tables are used to organize data into rows and columns. They are created using
the `<table>` element.

```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

Here, `<tr>` defines a table row, `<th>` defines a header cell, and `<td>`
defines a standard cell in the table. This table is used to represent data in a
structured format, which can be particularly useful for displaying tabular data
like schedules, statistics, or lists.

## CSS

### What is CSS?

CSS (Cascading Style Sheets) is a stylesheet language used to describe the
presentation of a document written in HTML. It allows you to control the layout,
colors, fonts, and other visual aspects of web pages.

### Why Should I Learn CSS?

CSS is essential for web development because it provides the styling and
aesthetic aspects of a webpage. It makes websites visually appealing and
improves the user experience.

### How to Apply Styles

**Inline**: Directly within an HTML element using the `style` attribute.

```html
<p style="color: red;">This is an inline style.</p>
```

**Internal**: Within the `<style>` tags in the HTML `<head>` section.

```html
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```

**External**: In a separate .css file that is linked to the HTML file.

```html
<link rel="stylesheet" href="styles.css" />
```

### Selectors

Selectors are patterns that match against elements in an HTML document, used to
apply styles.

**Type Selector**: Matches elements by node name.

    ```css
    p {
      color: green;
    }
    ```

**Class Selector**: Matches elements by class attribute.

    ```css
    .highlight {
      font-weight: bold;
    }
    ```

**ID Selector**: Matches a single element by its ID attribute.

    ```css
    #navbar {
      background-color: black;
    }
    ```

**Specificity**: Determines which CSS rule is applied when multiple rules could
apply to an element. It is calculated based on the different categories of
selectors.

- Inline styles have the highest specificity.
- ID selectors have higher specificity than class selectors.
- Class selectors have higher specificity than type selectors.

### Common CSS Properties

**Color**: Sets the text color.

```css
p {
  color: red;
}
```

**Text Alignment**: Aligns the text within an element.

```css
h1 {
  text-align: center;
}
```

**Font Size and Family**: Sets the font size and type for text.

```css
.text {
  font-size: 16px;
  font-family: Arial, sans-serif;
}
```

**Height and Width**: Sets the height and width of an element.

```css
.box {
  height: 100px;
  width: 200px;
}
```

**Border and Border Radius**: Sets the border style and radius (rounded
corners).

```css
.rounded-border {
  border: 2px solid blue;
  border-radius: 10px;
}
```

### Box Model

The CSS Box Model is the foundation of layout on the Web — each element is
represented as a rectangular box, with the box's content, padding, border, and
margin built up around one another like the layers of an onion.

**Content**: The actual content of the box, where text and images appear.
**Padding**: Clears an area around the content inside the border. It's
transparent. **Border**: A border that goes around the padding and content.
**Margin**: Clears an area outside the border.

Use padding when you want to create space within the element, and margin when
you want to create space between different elements.

```css
.div {
  content: "content";
  padding: 10px;
  border: 2px solid black;
  margin: 20px;
}
```

## Flexbox

CSS Flexbox, or Flexible Box Module, is a one-dimensional layout model that
allows you to design flexible and responsive layouts with ease.

### What is CSS Flexbox?

CSS Flexbox is a layout model designed for arranging items within a container in
a way that they can adjust their size and position to best utilize the available
space. It is particularly useful for building responsive designs and is a
powerful tool for aligning elements within a container.

### Benefits

- Flexibility: Automatically adjust the size of elements to fill the available
  space.
- Alignment Control: Easily vertically center elements, which was difficult
  before Flexbox.
- Responsiveness: Build designs that adapt to different screen sizes without
  complex code.

### Flex Container

To create a flex container, use the `display` property and set it to `flex`.

```css
.container {
  display: flex;
}
```

You can control the direction of the flex items by setting the `flex-direction`
property.

```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

### Flex Items

Flex items are the direct children of the flex container. You can control their
order and alignment within the container.

```css
.item {
  order: 2; /* Adjust the order */
  align-self: center; /* Align this item vertically in the center */
}
```

### Main Axis and Cross Axis

In a flex container, the main axis is the primary axis along which the flex
items are laid out, and the cross axis is perpendicular to it.

Use `justify-content` to align items along the main axis.

```css
.container {
  justify-content: center | flex-start | flex-end | space-between | space-around;
}
```

Use `align-items` and `align-self` to align items along the cross axis.

```css
.container {
  align-items: center | flex-start | flex-end | stretch | baseline;
}
```

### Flex Wrapping and Line Wrapping

Control how flex items wrap within the container using the `flex-wrap` property.

```css
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

### Flexbox Alignment

Use `align-content` to align items within flex lines and distribute extra space
among flex items with `flex-grow` and `flex-shrink`.

```css
.container {
  align-content: center | flex-start | flex-end | space-between | space-around |
    stretch;
}

.item {
  flex-grow: 2; /* Item will take up twice as much space as other items */
  flex-shrink: 1; /* Item can shrink if needed */
}
```

## Grid

CSS Grid is a powerful layout system that lets you create two-dimensional
layouts for web pages. With Grid, you can control both columns and rows, making
complex designs easier to achieve.

### What is CSS Grid?

CSS Grid is a layout model that allows developers to create complex responsive
web design layouts with ease. It excels at dividing a page into major regions or
defining the relationship in terms of size, position, and layer between parts of
the content.

### Benefits

- Precision: Provides precise control over the layout, irrespective of the
  screen size.
- Simplicity: Simplifies complex layouts that would be tough and hacky to
  achieve using other layout models.
- Flexibility: Easily create responsive designs without relying on external
  libraries like Bootstrap.

### Defining a Grid

To define an element as a grid container, use the `display` property and set it
to `grid`.

```css
.container {
  display: grid;
}
```

### Grid Template (Columns and Rows)

Using `grid-template-columns` and `grid-template-rows`, you can define the size
of the columns and rows of your grid.

```css
.container {
  grid-template-columns: 100px 200px 100px;
  grid-template-rows: 50px 50px;
}
```

### FR Unit

The `fr` unit represents a fraction of the available space in the grid
container. It is useful for creating responsive designs.

```css
.container {
  grid-template-columns: 1fr 2fr;
}
```

### Gaps Between Tracks

Use `gap`, `row-gap`, and `column-gap` to control the spacing between grid
cells.

```css
.container {
  gap: 10px;
  row-gap: 20px;
  column-gap: 20px;
}
```

### Repeating Track Listings

The `repeat()` function can be used to repeat the size of columns or rows
multiple times.

```css
.container {
  grid-template-columns: repeat(3, 100px);
}
```

### Minmax Function

The `minmax()` function defines a size range for grid tracks, allowing them to
have a minimum and maximum size.

```css
.container {
  grid-template-columns: minmax(100px, 1fr);
}
```

### Line-Based Placement

You can place grid items by referring to the lines that separate the grid
tracks, using `grid-column-start`, `grid-column-end`, `grid-row-start`, and
`grid-row-end`.

```css
.item {
  grid-column-start: 1;
  grid-column-end: 3;
  grid-row-start: 1;
  grid-row-end: 2;
}
```

### Media Queries

Media queries are used to apply different styles for different media
types/devices. Media queries can be used to check many things, such as the width
and height of the viewport and screen, the resolution of the device, etc.

```css
@media screen and (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

In this example, when the screen size is 600px or smaller, the background color
will change to light blue.

## JavaScript

### What is JavaScript?

JavaScript is a high-level, dynamic programming language primarily known for
adding interactivity and other complex features to websites. It is an essential
technology for web development, alongside HTML and CSS. However, it has evolved
over time and is now used for server-side development, mobile applications, and
even desktop applications.

### Why Should I Learn JavaScript?

- **Web Development**: JavaScript is fundamental for building interactive
  websites.
- **Versatility**: It can be used for both client-side and server-side
  development.
- **Community and Libraries**: There's a large community and countless libraries
  and frameworks available.

### Types of Values

JavaScript has various types of values, including:

- **Number**: Represents numeric values. e.g., `5`, `3.14`.
- **String**: Represents a sequence of characters. e.g., `"hello"`.
- **Boolean**: Represents a true or false value. **Object**: Represents a
  collection of key-value pairs.
- **Array**: Represents an ordered list of values.
- **Function**: Represents a reusable set of statements.
- **Null**: Represents an intentional absence of any value or object.
- **Undefined**: Represents a variable that has not been assigned a value.

Example:

```javascript
var num = 42; // Number
var text = "hello"; // String
var isActive = false; // Boolean
var obj = {}; // Object
var arr = [1, 2, 3]; // Array
```

### Type Conversion

In JavaScript, type conversion is the process of converting values from one data
type to another. This can happen automatically (implicit conversion) or be
performed explicitly using certain functions.

Example of implicit conversion: When you add a number and a string, JavaScript
converts the number to a string and concatenates them.

```javascript
var result = 5 + "7"; // "57" as a string, not 12
```

Using `parseInt()` to parse an integer from a floating-point number string:

```javascript
var numberString = "3.14";
var integerNumber = parseInt(numberString); // 3
```

Using `parseFloat()` to parse a floating-point number from a string:

```javascript
var numberString = "3.14";
var floatNumber = parseFloat(numberString); // 3.14
```

### Operators

- **Operand**: The value that the operator operates on.
- **Unary Operator**: Operates on a single operand. e.g., `!true` (logical NOT),
  `-x` (negation).
- **Binary Operator**: Operates on two operands. e.g., `x + y` (addition),
  `x < y` (less than).

Example:

```javascript
var x = 10;
var y = 5;

// Unary
var negativeX = -x; // -10

// Binary
var sum = x + y; // 15
```

### Modifying Variables in Place

You can modify variables in place using various operators:

- `++` : Increment
- `--` : Decrement
- `+=`, `-=`: Change value in place

Example:

```javascript
var counter = 0;
counter++; // Increment by 1
counter--; // Decrement by 1
counter += 5; // Increase by 5
```

### Comparisons

Comparison operators are used to compare values:

- `==`: Equality (does not check the type)
- `===`: Strict equality (checks both value and type)
- `<`, `>`, `<=`, `>=`: Comparisons

Example:

```javascript
var age = 30;

if (age >= 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}
```

### Conditionals

Conditionals are used to make decisions in code:

- `if`: Execute block if the condition is true.
- `else if`: Execute block if the previous condition was false and the current
  condition is true.
- `else`: Execute block if none of the above conditions is true.

Example:

```javascript
var score = 85;

if (score >= 90) {
  console.log("A");
} else if (score >= 80) {
  console.log("B");
} else {
  console.log("C");
}
```

### Loops

Loops are used to execute a block of code repeatedly:

- `for`: Execute code a specific number of times.
- `while`: Execute code as long as a condition is true.
- `do...while`: Execute code at least once, and then as long as a condition is
  true.

Example:

```javascript
// for loop
for (var i = 0; i < 5; i++) {
  console.log(i); // 0, 1, 2, 3, 4
}

// while loop
var j = 0;
while (j < 5) {
  console.log(j); // 0, 1, 2, 3, 4
  j++;
}
```

### Functions

Functions are reusable blocks of code that can be defined once and used multiple
times:

**Declaration**: Define a function using the `function` keyword. **Parameters**:
The inputs to the function. **Return**: Send a value back to the caller. **Local
variables**: Variables defined inside the function - not accessible outside.
**Outer variables**: Variables defined outside the function - accessible inside.

Example:

```javascript
function add(a, b) {
  var sum = a + b;
  return sum;
}

var result = add(5, 10); // 15
console.log(result); // 15
```

### Arrays

Arrays are used to store multiple values in a single variable:

- **Length**: Find out how many elements are in an array with `.length`.
- **Filtering**: Create a new array with elements that pass a test with
  `.filter()`.
- **Mapping**: Create a new array by transforming every element in an array with
  `.map()`.

Example:

```javascript
var numbers = [1, 2, 3, 4, 5];

// Length
console.log(numbers.length); // 5

// Filtering
var evenNumbers = numbers.filter(function (num) {
  return num % 2 === 0;
});
console.log(evenNumbers); // [2, 4]

// Mapping
var squares = numbers.map(function (num) {
  return num * num;
});
console.log(squares); // [1, 4, 9, 16, 25]
```

### Objects

Objects in JavaScript are collections of key-value pairs, where the keys are
strings and the values can be any data type, including functions. Objects are
used to store structured data and represent real-world entities.

#### Creating Objects

You can create an object using curly braces `{}`.

```javascript
let person = {
  name: "John",
  age: 25,
};
```

#### Accessing Properties

You can access the properties of an object using the dot notation.

```javascript
console.log(person.name); // Output: "John"
```

Alternatively, you can use the square brackets notation. This is particularly
useful when the property name is stored in a variable or if the property name is
not a valid identifier.

```javascript
console.log(person["age"]); // Output: 25

let propertyName = "name";
console.log(person[propertyName]); // Output: "John"
```

#### Adding Functions to Objects

Objects can also store functions. These functions are often referred to as
methods when they are properties of an object.

```javascript
let person = {
  name: "Alice",
  age: 30,
  greet: function () {
    console.log("Hello, " + this.name);
  },
};

person.greet(); // Output: "Hello, Alice"
```

In the example above, `greet` is a method of the `person` object. The `this`
keyword inside the `greet` method refers to the `person` object.

### `this`

In JavaScript, the `this` keyword is a special identifier that's automatically
defined in the scope of every function. It refers to the object on which the
function was called, also known as the calling object. The value of `this` is
determined based on how the function is called.

#### In a Method

When a function is a property of an object (a method), `this` refers to the
object itself.

```javascript
let person = {
  name: "Alice",
  greet: function () {
    console.log("Hello, my name is " + this.name);
  },
};

person.greet(); // Output: "Hello, my name is Alice"
```

#### In a Regular Function

In a regular function (not an arrow function), `this` doesn't refer to the
enclosing object literal. Instead, in non-strict mode, it defaults to the global
object (`window` in browsers), while in strict mode, it's `undefined`.

```javascript
function showThis() {
  console.log(this);
}

showThis(); // In non-strict mode: Output is the global object. In strict mode: Output is undefined.
```

#### In an Arrow Function

Arrow functions don’t have their own `this`. Instead, `this` is lexically bound
to the enclosing scope.

```javascript
let person = {
  name: "Alice",
  greet: () => {
    console.log("Hello, my name is " + this.name);
  },
};

person.greet(); // Output: "Hello, my name is undefined" because `this` is not bound to the person object
```

#### Using `this` in an Event Listener

In an event listener, `this` refers to the DOM element that is the target of the
event.

```javascript
button.addEventListener("click", function () {
  console.log(this); // Output: the DOM element targeted by the event
});
```

#### Changing the Value of `this`

```javascript
function greet() {
  console.log("Hello, " + this.name);
}

let person1 = { name: "Alice" };
let person2 = { name: "Bob" };

greet.call(person1); // Output: "Hello, Alice"
greet.call(person2); // Output: "Hello, Bob"
```

### Constructor and "new" Operator

Constructors are functions used to create objects with a specific structure and
behavior. The `new` operator is used to create an instance of an object using a
constructor.

In constructors, the `this` keyword refers to the instance of the object being
created.

Example:

```javascript
function User(name, age) {
  this.name = name; // 'this' refers to the instance of User
  this.age = age;
}

var user = new User("John", 30);

console.log(user.name); // Output: "John"
console.log(user.age); // Output: 30
```

In the above example, `this` refers to the object that's being created by the
constructor function. It allows you to set properties on the object, which can
then be accessed using the dot notation.

### Arrow Functions

Arrow functions provide a shorter syntax for writing functions.

Here's an example of a function written the "regular way":

```javascript
function add(a, b) {
  return a + b;
}
```

Here's the same function using an arrow function:

```javascript
const add = (a, b) => {
  a + b;
};
```
