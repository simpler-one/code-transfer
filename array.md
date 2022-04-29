# Array / List
## Copy(shallow)
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const result = [...source];
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
result = source.copy()
```
---
```python
result = source[:]
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
int[] result = Arrays.copyOf(source, source.length);
```
---
```java
int[] result = new int[source.length];
System.arraycopy(source, 0, result, 0, source.length);
```
---
```java
List<T> result = new ArrayList<>(source);
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
T[] result = new T[source.Length];
source.CopyTo(result, 0);
```
---

```c#
T[] result = new T[source.Length];
Array.Copy(source, 0, result, 0, source.Length);
```
---
```c#
T[] result = <T[]>source.Clone();
```
</td></tr>
</tbody></table>


## Map
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const result = source.map(v => v * 2);
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
result = [v * 2 for v in source]
```
---
```python
result = list(map(lambda v: v * 2, source))
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
List<Integer> result = source.stream().map(v -> v * 2).collect(Collectors.toList());
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
T[] result = Array.ConvertAll(source, v => v * 2);
```
---
```c#
using System.Linq;
...
T[] result = source.Select(v => v * 2).ToArray();
```
</td></tr>
</tbody></table>


## Filter
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const result = source.filter(v => v !== undefined);
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
result = [v for v in source if v is not None]
```
---
```python
result = list(filter(lambda v: v is not None, source))
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
List<Integer> result = source.stream()
    .filter(v -> v != null)
    .collect(Collectors.toList())
;
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
T[] result = Array.FindAll(source, v => v != null);
```
---
```c#
using System.Linq;
...
T[] result = source.Where(v => v != null).ToArray();
```
</td></tr>
</tbody></table>


## Find
<table><tbody>
<tr><td valign="middle">JavaScript</td><td>

```js
const result = source.find(v => v !== undefined);
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
result = next((v for v in source if v is not None), None)
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
List<Integer> result = source.stream()
    .filter(v -> v != null)
    .findFirst()
    .orElse(null)
;
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
T result = Array.Find(source, v => v != null);
```
---
```c#
using System.Linq;
...
T result = source.FirstOrDefault(v => v != null);
```
</td></tr>
</tbody></table>
