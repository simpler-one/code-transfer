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


## Format(space padding)
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
text = f"price: {price: >6}"
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


## Format(zero padding)
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const year = "1234".padStart(4, "0");
const month = "5".padStart(2, "0");
const day = "6".padStart(2, "0");
const date = `${year}-${month}-${day}`;
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
year = 1234
month = 5
day = 6
date = f"{year:0>4}-{month:0>2}-{day:0>2}"
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
String year = "1234";
String month = "5";
String day = "6";
String date = String.format("%4s-%2s-%2s", year, month, day);
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
string year = "1234".PadLeft(4, '0');
string month = "5".PadLeft(2, '0');
string day = "6".PadLeft(2, '0');
string date = $"{year}-{month}-{day}";
```
</td></tr>
</tbody></table>


## Format(figure)
TODO
