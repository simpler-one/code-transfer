# Array / List
## Copy(shallow)
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const copy = [...array]
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
copy = array.copy()
```
---
```python
copy = array[:]
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
int[] copy = ?;
```
---
```java
List<T> copy = ?;
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
T[] copy = new T[array.Length];
array.CopyTo(copy, 0);
```
---

```c#
T[] copy = new T[array.Length];
Array.Copy(array, 0, copy, 0, array.Length);
```
</td></tr>
</tbody></table>
