# String
## Template literal
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const name = "Tom";
const value = "a boy";
const text = `${name} is ${value}`;
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
domain = "abc.example.dom"
path = "foo/bar"
url = f"https://{domain}/{path}"
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
String predicate = "not old-fashioned"
String text = String.format("Java is %s", predicate);
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
string name = "World";
string text = $"Hello {name}"
```
</td></tr>
</tbody></table>


## Padding
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const price = "123";
const text = `price: ${price.padStart(6, " ")}`;
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
price = 123
url = f"price: {price: >6}"
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
String price = "123";
String text = String.format("price: %6s", price);
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
string price = "123";
string text = $"price: {price.PadLeft(6, ' ')}";
```
</td></tr>
</tbody></table>
