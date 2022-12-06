# The Zen of Python
## By Tim Peters

[comment]: # (||| data-background-color="hsl(0, 100%, 75%)")

... as a slideshow by Jonatan Skogsfors

[comment]: # (!!! data-background-color="hsl(0, 100%, 75%)")

# Beautiful is better than ugly.

[comment]: # (||| data-auto-animate data-background-color="hsl(18, 100%, 75%)")
Beautiful is better than ugly.
```python
# Don't

def powers(l):
    p = []
    for i in range(len(l)):
        p.append(l[i] * l[i])
    return p
```
<!-- .element: data-id="code" -->

[comment]: # (||| data-auto-animate data-background-color="hsl(18, 100%, 75%)")
Beautiful is better than ugly.
```python
# Do

def calculate_powers(numbers: list[int]) -> list[int]:
    return [number ** 2 for number in numbers]
```
<!-- .element: data-id="code" -->

[comment]: # (!!! data-auto-animate data-background-color="hsl(18, 100%, 75%)")

# Explicit is better than implicit.

[comment]: # (!!!  data-background-color="hsl(36, 100%, 75%)")

# Simple is better than complex.

[comment]: # (!!! data-background-color="hsl(54, 100%, 75%)")

# Complex is better than complicated.

[comment]: # (!!! data-background-color="hsl(72, 100%, 75%)")

# Flat is better than nested.

[comment]: # (!!! data-background-color="hsl(90, 100%, 75%)")

# Sparse is better than dense.

[comment]: # (!!! data-background-color="hsl(108, 100%, 75%)")

# Readability counts.

[comment]: # (||| data-background-color="hsl(126, 100%, 75%)")
Readability counts.
```python
    def f(x, y):
        pass
```
<!-- .element: data-id="code" -->
[comment]: # (||| data-auto-animate data-background-color="hsl(126, 100%, 75%)")
Readability counts.
```python
    def calculate_cost(price, count):
        return price * count
```
<!-- .element: data-id="code" -->
[comment]: # (||| data-auto-animate data-background-color="hsl(126, 100%, 75%)")
Readability counts.
```python
    def calculate_cost(price: int, count: int) -> int:
        return price * count
```
<!-- .element: data-id="code" -->
[comment]: # (!!! data-auto-animate data-background-color="hsl(126, 100%, 75%)")

# Special cases aren't special enough to break the rules.

[comment]: # (!!! data-background-color="hsl(144, 100%, 75%)")

# Although practicality beats purity.

[comment]: # (!!! data-background-color="hsl(162, 100%, 75%)")

# Errors should never pass silently.

[comment]: # (!!! data-background-color="hsl(180, 100%, 75%)")

# Unless explicitly silenced.

[comment]: # (!!! data-background-color="hsl(198, 100%, 75%)")

# In the face of ambiguity, refuse the temptation to guess.

[comment]: # (!!! data-background-color="hsl(216, 100%, 75%)")

# There should be one-- and preferably only one --obvious way to do it.

[comment]: # (!!! data-background-color="hsl(234, 100%, 75%)")

# Although that way may not be obvious at first unless you're Dutch.

[comment]: # (!!! data-background-color="hsl(252, 100%, 75%)")

# Now is better than never.

[comment]: # (!!! data-background-color="hsl(270, 100%, 75%)")

# Although never is often better than *right* now.

[comment]: # (!!! data-background-color="hsl(288, 100%, 75%)")

# If the implementation is hard to explain, it's a bad idea.

[comment]: # (!!! data-background-color="hsl(306, 100%, 75%)")

# If the implementation is easy to explain, it may be a good idea.

[comment]: # (!!! data-background-color="hsl(324, 100%, 75%)")

# Namespaces are one honking great idea -- let's do more of those!

[comment]: # (||| data-background-color="hsl(342, 100%, 75%)")
Namespaces are one honking great idea -- let's do more of those!
```python
from foo import *
from bar import baz

x = calculate(42)
y = baz(x)
```
<!-- .element: data-id="code" -->
[comment]: # (||| data-auto-animate data-background-color="hsl(342, 100%, 75%)")
Namespaces are one honking great idea -- let's do more of those!
```python
import foo
import bar

x = foo.calculate(42)
y = bar.baz(x)
```
<!-- .element: data-id="code" -->
[comment]: # (!!! data-auto-animate data-background-color="hsl(342, 100%, 75%)")
