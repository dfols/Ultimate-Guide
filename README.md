## Ultimate Study Guide

### Command Line Interface (CLI)

#### What is CLI?

The Command Line Interface (CLI) is a user interface that allows you to interact
with your computer using text-based commands.

#### Why Should I Learn Command Line?

- Direct interaction with the operating system.
- Automating tasks using scripts.
- Essential for software development and system administration.

#### Shell vs. Bash vs. Terminal vs. Command Prompt

- **Shell**: A program that interprets text-based commands.
- **Bash (Bourne Again Shell)**: A popular shell that supports scripting and
  command-line editing.
- **Terminal**: A program that allows you to use the shell.
- **Command Prompt**: Windows equivalent of the terminal.

#### Common Commands

- `cd`: Change Directory.
- `ls`: List files and directories.
- `mkdir`: Make a directory.
- `rm`: Remove files or directories.

### HTML

#### What is HTML?

HTML (HyperText Markup Language) is the standard markup language for creating
web pages.

#### Why Should I Learn HTML?

- Foundation for web development.
- Structure and content of web pages.
- Embed images, audio, video, and interactive forms.

#### How an Element is Structured

```
<tagname attribute="value">Content</tagname>
```

#### Document Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <!-- Page content -->
  </body>
</html>
```

#### Inline vs. Block

- **Inline**: Elements that do not take up the full width of the page. e.g.
  `<span>`
- **Block**: Elements that take up the full width of the page. e.g. `<div>`

#### Semantic HTML

Semantic HTML elements convey meaning and structure. Example: `<header>`,
`<nav>`, `<section>`, `<article>`.

#### Text Formatting Tags

- `<p>`: Paragraph
- `<h1>` to `<h6>`: Headings
- `<em>`: Emphasis (typically italic)
- `<strong>`: Bold
- `<u>`: Underline
- `<ol>`: Ordered List
- `<ul>`: Unordered List

#### Links

`<a href="url">Link text</a>`

#### Images

`<img src="image.jpg" alt="description">`

#### Forms and Inputs

```html
<form>
  <input type="text" name="name" />
  <input type="submit" value="Submit" />
</form>
```

#### Tables

```html
<table>
  <tr>
    <th>Header</th>
  </tr>
  <tr>
    <td>Data</td>
  </tr>
</table>
```

### CSS

#### What is CSS?

CSS (Cascading Style Sheets) is a language used to describe the style of HTML
documents.

#### Why Should I Learn CSS?

- Enhance the appearance of web pages.
- Control layout, colors, fonts, and more.
- Adaptive designs for different devices.

#### Where to Put CSS

1. **Inline**: Within an HTML element.
2. **Internal**: Within the `<style>` tags in the `<head>` section.
3. **External**: Link to an external `.css` file.

#### Selectors and Specificity

- **Selectors**: Patterns used to select elements. e.g. `.class`, `#id`,
  `element`.
- **Specificity**: Rules for resolving conflicts between styles.

#### Common CSS Properties

- `color`
- `text-align`
- `font-size`
- `font-family`
- `width`, `height`
- `border`, `

border-radius`

- `margin`, `padding`

#### Box Model

Content > Padding > Border > Margin

#### Flexbox

- `display: flex`
- `justify-content`
- `align-items`, `align-content`
- `flex-direction`
- `flex-grow`, `flex-shrink`, `flex-basis`

#### Grid

- `display: grid`
- `grid-template-columns`, `grid-template-rows`
- `grid-column`, `grid-row`

#### Media Queries

- Responsive design based on screen size.
- Example: `@media (max-width: 600px) { … }`

### Git

#### What is Git?

Git is a distributed version control system for tracking changes in source code.

#### Why Should I Learn Git?

- Collaborate on code with others.
- Keep a history of changes.
- Merge code and resolve conflicts.

#### Git vs. GitHub

- **Git**: The version control system.
- **GitHub**: A web-based platform for hosting Git repositories.

#### Basic Git Commands

- `git init`: Initialize a new Git repository.
- `git add`: Stage changes for commit.
- `git commit`: Commit staged changes.
- `git push`: Push commits to a remote repository.
- `git pull`: Fetch and integrate changes from a remote repository.
- `git branch`: List, create, or delete branches.

### JavaScript

As you've already provided a template for JavaScript, I'll focus on additional
topics.

#### Types of Values

- Number
- String
- Boolean
- Object
- Array
- Function
- Null
- Undefined

#### Type Conversion

Conversion between different types, e.g. string to number. `parseInt()`,
`parseFloat()`.

#### Unary, Binary, Operand

- **Unary** - Single operand. e.g., `!true`, `-x`.
- **Binary** - Two operands. e.g., `x + y`, `x < y`.
- **Operand** - The value operated on.

#### Modifying Variables in Place

- `++`, `--` : Increment or decrement
- `+=`, `-=`, etc: Change value in place

#### Comparisons

- `==`: Equality
- `===`: Strict equality
- `<`, `>`, `<=`, `>=`: Comparisons

#### Conditionals

- `if`, `else if`, `else`
- Ternary operator `?`

#### Loops

- `for`
- `while`
- `do...while`

#### Functions

- **Declaration**: `function myFunc() { ... }`
- **Parameters**: The names listed in the function definition.
- **Return**: Stop function and return value.
- **Local variables**: Variables defined inside function.
- **Outer variables**: Variables outside function but accessible.

#### Function is a Value

Functions can be assigned to variables, passed as arguments, and returned from
other functions.

#### Callback Functions

A function passed into another function as an argument.

#### Function Expression vs Function Declaration

- **Function Expression**: `var myFunc = function() { ... }`
- **Function Declaration**: `function myFunc() { ... }`

#### Array Methods

- `filter()`
- `map()`
- `length`

#### Objects

- **Properties and Values**: `obj.prop = value`.
- **Square Brackets Notation**: `obj["prop"]`.
- **Property Existence Test**: `"prop" in obj`.
- **For...in Loop**: Loop through properties.
- **`this` in methods**: Access object.
- **Arrow Functions and `this`**: Arrow functions do not have their own `this`.

#### Constructor and "new" Operator

- Creating instances of custom object types.

```javascript
function User(name) {
  this.name = name;
}

var user = new User("John");
```

This guide should serve as a comprehensive overview of the topics you covered in
your coding bootcamp. Happy coding!
