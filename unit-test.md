# Unit test
## Elementary
<table><tbody>
<tr><td valign="middle">JavaScript/Jest(describe)</td><td>

```js
describe("Foo", () => {
    describe("answer()", () => {
        it("should return 42 if question is string", () => {
            // given
            question = "Life, the Universe, and Everything";
            instance = new Foo();

            // when
            result = instance.answer(question);

            // then
            expect(result).toEqual(42);
        });

        it("should return null if question is null", () => {
            ...
        });
    });
});
```
</td></tr>

<tr><td valign="middle">Python/pytest</td><td>

```python
class TestDoSomething:
    def test_str_question(self):
        # given
        question = "Life, the Universe, and Everything"
        instance = Foo()

        # when
        result = instance.answer(question)

        # then
        assert result == 42

    def test_none_question(self):
        ...
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
// TODO
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
// TODO
```
</td></tr>
</tbody></table>


## Mock function
<table><tbody>
<tr><td valign="middle">JavaScript/Jest(describe)</td><td>

```js
// TODO
```
</td></tr>

<tr><td valign="middle">Python/pytest</td><td>

```python
# TODO
```
</td></tr>

<tr><td valign="middle">Java</td><td>

```java
// TODO
```
</td></tr>
<tr><td valign="middle">C#</td><td>

```c#
// TODO
```
</td></tr>
</tbody></table>


## Preprocess/Postprocess
TODO

