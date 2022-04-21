# Generic
## Class
<table><tbody>
<tr><td valign="middle">TypeScript</td><td>

```ts
class Foo<T> {
    value: T;
}

const foo = new Foo<Bar>()
```
</td></tr>

<tr><td valign="middle">JavaScript</td><td>

```js
/**
 * @template T
 */
class Foo {
    /** @type {T} */
    value;
}

/** @type {Foo<Bar>} */
const foo = new Foo()
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
from typing import Generic, TypeVar
T = TypeVar("T")


class Foo(Generic[T]):
    @property
    def value(self) -> T:
        pass

foo = Foo[Bar]()
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
class Foo<T> {
    T value;
}

Foo<T> foo = new Foo<>();
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
class Foo<T> {
    T value;
}

Foo<T> foo = new Foo():
```
</td></tr>
</tbody></table>


## Function
<table><tbody>
<tr><td valign="middle">TypeScript</td><td>

```ts
function foo<T>(value: T): void { /* do something */ }

foo<Bar>(bar);
```
---
```ts
const foo<T> = (value: T) => { /* do something */ }

foo<Bar>(bar);
```
</td></tr>

<tr><td valign="middle">Python</td><td>

```python
from typing import TypeVar
T = TypeVar("T")


def foo(value: T) -> None:
    pass
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
class Foo {
    <T> void foo(T value) { /* do something */ }
}

fooInstance.<Bar>foo(bar);
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
class Foo {
    void foo<T>(T value) { /* do something */ }
}

fooInstance.foo<Bar>(bar);
```
</td></tr>
</tbody></table>
