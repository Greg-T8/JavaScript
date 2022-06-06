# JavaScript Fundamentals
**Reference:**
- https://javascript.info/first-steps

## Hello, World!
**Reference**
- https://javascript.info/hello-world

The simplest way to create a Hello World script is to use the `<script>` tag:

```HTML
<!DOCTYPE html>
<html>
  <body>
    <p>Before the script...</p>
    
    <script>
      alert( 'Hello, world!');
    </script>

    <p>...After the script.</p>
  </body>
</html>
```

This prints out the following message:

&emsp;![](img/1-1.png)

Alternatively, you can place the code `alert ('Hello, world!")` in a separate file and reference it:

```HTML
<!DOCTYPE html>
<html>
  <body>
    <p>Before the script...</p>
    
    <script src="assets/script.js"></script>

    <p>...After the script.</p>
  </body>
</html>
```

## Code Structure
**Reference**
- https://javascript.info/structure

### Statements
Statements are typically written on separate lines to make the code more readable. Semicolons may be omitted in most cases where a line break exists:

```JavaScript
alert('Hello')
alert('World')
```
In most cases a newline implies a semicolon, but there are cases where a newline doesn't mean a semicolon:
```JavaScript
alert(3 +
1
+ 2);
```
In the code above, JavaScript understands the "+" indicates an incomplete expression, and does not apply a semicolon. However, there are situations where JavaScript fails to assume a semicolon where it is really needed, so the **authors recommend putting semicolons between statements even if they are separated by newlines**.

### Comments
One-line comments start with two forward slash characters `//`:
```JavaScript
// This comment occupies a line of its own
alert (Hello);
```

Multiline comments start w/ a forward slash and an asterisk `/*` and end with an asterisk and a forward slash `*/`:
```JavaScript
/* An example with two messages.
This is a multiline comment.
*/
alert('Hello');
```
