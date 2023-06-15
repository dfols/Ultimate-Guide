## Ultimate Study Guide

### Command Line Interface (CLI)

#### What is CLI?

The Command Line Interface (CLI) is a user interface that allows you to interact
with your computer using text-based commands.

#### Why Should I Learn Command Line?

- Direct interaction with the operating system.
- Automating tasks using scripts.
- Essential for software development and system administration.

#### Shell vs. Terminal

- **Shell**: A shell is a program that processes commands and returns output.
  It's an interface that allows users to interact with the operating system by
  entering commands. Shells can be interactive or used to execute scripts.

- **Terminal**: A terminal, also known as a terminal emulator, is a program that
  provides the text-based interface to the shell. The terminal emulates a
  console, allowing users to type in shell commands. It sends the commands to
  the shell for processing and then displays the output. The terminal itself
  doesn't handle command processing; it's just the interface to the shell.

#### Common Commands

- `cd`: Change Directory.
- `ls`: List files and directories.
- `pwd`: Print Working Directory - shows the current directory path.
- `mkdir`: Make a directory.
- `rmdir`: Remove an empty directory.
- `rm`: Remove files or directories.
- `cp`: Copy files or directories.
- `mv`: Move files or directories.
- `echo`: Display a line of text.
- `cat`: Display the content of files.
- `grep`: Search for a specific pattern within a file.
- `sudo`: Execute a command with superuser permissions.
- `man`: Display the user manual for a command.

#### Example Workflow:

Here is an example workflow combining the commands above:

```sh
mkdir my_new_directory      # Create a new directory named "my_new_directory"
cd my_new_directory         # Change directory to the newly created directory
touch example.txt           # Create a new file named "example.txt" in the current directory
```

### HTML

#### What is HTML?

HTML (Hypertext Markup Language) is the standard markup language for documents
designed to be displayed in a web browser. It helps structure the content and
present it on the web.

#### Why Should I Learn HTML?

HTML is the backbone of web pages. Learning HTML is essential for anyone
interested in web development or design, as it's the basic building block for
creating websites.

#### Document Structure

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

#### Inline vs Block Elements

- **Inline Elements**: Do not start on a new line and only take up as much width
  as necessary. Example: `<span>`, `<a>`.

  ```html
  This is <span>inline</span> element.
  ```

- **Block Elements**: Start on a new line and take up the full width available.
  Example: `<div>`, `<h1>`, `<p>`.

  ```html
  <div>This is a block element.</div>
  ```

#### Semantic HTML

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

#### Links

Links are used to navigate between pages on the internet. The `<a>` tag is used
to create hyperlinks.

- Basic link example:

  ```html
  <a href="https://example.com">This is a link</a>
  ```

- Open link in a new tab:

  ```html
  <a href="https://example.com" target="_blank">Open in new tab</a>
  ```

#### Forms and Inputs

Forms are essential for collecting data from the user. The `<form>` element acts
as a container for different types of input elements such as text fields,
checkboxes, radio buttons, and buttons.

```html
<form action="/submit_form" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" /><br />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" /><br />

  <input type="submit" value="Submit" />
</form>
```

#### Tables

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

### CSS

#### What is CSS?

CSS (Cascading Style Sheets) is a stylesheet language used to describe the
presentation of a document written in HTML. It allows you to control the layout,
colors, fonts, and other visual aspects of web pages.

#### Why Should I Learn CSS?

CSS is essential for web development because it provides the styling and
aesthetic aspects of a webpage. It makes websites visually appealing and
improves the user experience.

#### Where to Put CSS

- **Inline**: Directly within an HTML element using the `style` attribute.

  ```html
  <p style="color: red;">This is an inline style.</p>
  ```

- **Internal**: Within the `<style>` tags in the HTML `<head>` section.

  ```html
  <head>
    <style>
      p {
        color: blue;
      }
    </style>
  </head>
  ```

- **External**: In a separate .css file that is linked to the HTML file.

  ```html
  <link rel="stylesheet" href="styles.css" />
  ```

#### Selectors and Specificity

- **Selectors**: Selectors are patterns that match against elements in an HTML
  document, used to apply styles.

  - **Type Selector**: Matches elements by node name.

    ```css
    p {
      color: green;
    }
    ```

  - **Class Selector**: Matches elements by class attribute.

    ```css
    .highlight {
      font-weight: bold;
    }
    ```

  - **ID Selector**: Matches a single element by its ID attribute.

    ```css
    #navbar {
      background-color: black;
    }
    ```

- **Specificity**: Determines which CSS rule is applied when multiple rules
  could apply to an element. It is calculated based on the different categories
  of selectors.
  - Inline styles have the highest specificity.
  - ID selectors have higher specificity than class selectors.
  - Class selectors have higher specificity than type selectors.

#### Common CSS Properties

- **Color**: Sets the text color.

  ```css
  p {
    color: red;
  }
  ```

- **Text Alignment**: Aligns the text within an element.

  ```css
  h1 {
    text-align: center;
  }
  ```

- **Font Size and Family**: Sets the font size and type for text.

  ```css
  .text {
    font-size: 16px;
    font-family: Arial, sans-serif;
  }
  ```

- **Height and Width**: Sets the height and width of an element.

  ```css
  .box {
    height: 100px;
    width: 200px;
  }
  ```

- **Border and Border Radius**: Sets the border style and radius (rounded
  corners).

  ```css
  .rounded-border {
    border: 2px solid blue;
    border-radius: 10px;
  }
  ```

#### Box Model

The CSS Box Model is the foundation of layout on the Web — each element is
represented as a rectangular box, with the box's content, padding, border, and
margin built up around one another like the layers of an onion.

- **Content**: The actual content of the box, where text and images appear.
- **Padding**: Clears an area around the content inside the border. It's
  transparent.
- **Border**: A border that goes around the padding and content.
- **Margin**: Clears an area outside the border.

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

#### Flexbox

Flexbox is a layout model that allows elements within a parent container to be
automatically arranged dynamically according to size and screen space.

- **Display**: To use flexbox, you need to set the parent element's display
  property to flex.

  ```css
  .flex-container {
    display: flex;
  }
  ```

- **Justify Content**: Aligns content horizontally.

  ```css
  .flex-container {
    justify-content: center;
  }
  ```

- **Align Items**: Aligns items vertically within a container.

  ```css
  .flex-container {
    align-items: center;
  }
  ```

- **Flex Direction**: Sets the direction of the flex items.

  ```css
  .flex-container {
    flex-direction: row | row-reverse | column | column-reverse;
  }
  ```

#### Grid

CSS Grid is a layout system that lets you design complex layouts by placing
elements into rows and columns.

```css
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-gap: 10px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 20px;
}
```

#### Media Queries

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

### Git

#### What is Git?

Git is a distributed version control system for tracking changes in source code.
It allows multiple developers to work on the same codebase without overwriting
each other's changes. Git stores code history, so you can revert to previous
versions if needed.

#### Why Should I Learn Git?

- **Collaborate on code with others**: Git enables multiple developers to work
  on the same project simultaneously.
- **Keep a history of changes**: You can view the history, find out who made
  which changes, and revert to a previous state if necessary.
- **Merge code and resolve conflicts**: Combine code from different branches and
  resolve conflicts when they arise.

#### Git vs. GitHub

- **Git**:
  - It is a version control system.
  - You can use Git locally on your computer.
  - Git helps you manage the history and collaboration of your code.
- **GitHub**:
  - GitHub is a web-based platform.
  - It uses Git for version control.
  - You can host your Git repositories online on GitHub.
  - It provides additional features like Pull Requests, Issues, and a web-based
    interface for repository management.

While Git is essential for version control, GitHub adds an extra layer of
functionality, particularly for collaboration across teams and the open-source
community.

#### Basic Git Commands with Examples

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

  Here, `origin` is the default name Git gives to the server you cloned from,
  and `main` is the branch you are pushing to.

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

#### Understanding Origin

In Git, `origin` is the default name given to the remote repository where you
want to publish your commits. It's essentially a shorthand name for the remote
repository's URL. For example, when you run the command `git push origin main`,
you're telling Git to push your changes to the main branch on the remote
repository associated with `origin`.

#### Working with Branches

Branches are used for developing features isolated from each other. The `main`
branch is the default branch when you create a repository. Use other branches
for development and merge them back to the `main` branch upon completion.

Example:

```sh
git checkout -b feature-branch # Create and switch

 to a new branch named "feature-branch"
# Make changes and commit them
git checkout main              # Switch back to the main branch
git merge feature-branch       # Merge the feature branch into the main branch
```

This workflow is a fundamental aspect of version control, allowing for parallel
development without conflicts.

### JavaScript

#### What is JavaScript?

JavaScript is a high-level, dynamic programming language primarily known for
adding interactivity and other complex features to websites. It is an essential
technology for web development, alongside HTML and CSS. However, it has evolved
over time and is now used for server-side development, mobile applications, and
even desktop applications.

#### Why Should I Learn JavaScript?

- **Web Development**: JavaScript is fundamental for building interactive
  websites.
- **Versatility**: It can be used for both client-side and server-side
  development.
- **Community and Libraries**: There's a large community and countless libraries
  and frameworks available.

#### Types of Values

JavaScript has various types of values, including:

- **Number**: Represents numeric values. e.g., `5`, `3.14`.
- **String**: Represents a sequence of characters. e.g., `"hello"`.
- **Boolean**: Represents a true or false value.
- **Object**: Represents a collection of key-value pairs.
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

#### Type Conversion

JavaScript allows you to convert between different types. For example:

- `parseInt("123")` converts the string `"123"` to the number `123`.
- `parseFloat("3.14")` converts the string `"3.14"` to the number `3.14`.
- `String(123)` converts the number `123` to the string `"123"`.

#### Operators

- **Unary Operator**: Operates on a single operand. e.g., `!true` (logical NOT),
  `-x` (negation).
- **Binary Operator**: Operates on two operands. e.g., `x + y` (addition),
  `x < y` (less than).
- **Operand**: The value that the operator operates on.

Example:

```javascript
var x = 10;
var y = 5;

// Unary
var negativeX = -x; // -10

// Binary
var sum = x + y; // 15
```

#### Modifying Variables in Place

You can modify variables in place using various operators:

- `++` : Increment
- `--` : Decrement
- `+=`, `-=`, etc: Change value in place

Example:

```javascript
var counter = 0;
counter++; // Increment by 1
counter += 5; // Increase by 5
```

#### Comparisons

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

#### Conditionals

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

#### Loops

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

#### Functions

Functions are reusable blocks of code that can be defined once and used multiple
times:

- **Declaration**: Define a function using the `function` keyword.
- **Parameters**: The inputs to the function.
- **Return**: Send a value back to the caller.
- **Local variables**: Variables defined inside the function - not accessible
  outside.
- **Outer variables**: Variables defined outside the function - accessible
  inside.

Example:

```javascript
function add(a, b) {
  var sum = a + b;
  return sum;
}

var result = add(5, 10); // 15
console.log(result); // 15
```

#### Arrays

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

#### Objects

Objects are collections of key-value pairs. They can store data and functions.

Example:

```javascript
var person = {
  name: "Alice",
  age: 30,
  greet: function () {
    console.log("Hello, " + this.name);
  },
};

console.log(person.name); // Alice
person.greet(); // Hello, Alice
```

#### Arrow Functions

Arrow functions allow for a shorter syntax when writing functions and do not
have their own `this` value.

Example:

```javascript
var add = (a, b) => a + b;

console.log(add(5, 10)); // 15
```

#### Constructor and "new" Operator

Constructors are used to create objects. The `new` operator is used to create an
instance of an object.

Example:

```javascript
function User(name) {
  this.name = name;
}

var user = new User("John");
console.log(user.name); // John
```
