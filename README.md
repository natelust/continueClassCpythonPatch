# Continue Class Patch

This patch introduces new syntax into python to address issues with, and clarify the process of, extending a class after the initial declaration. The following both shows the new syntax and provides a test for the patch.

```python
# Define a class Foo, taking a message as an argument
class Foo:
    def __init__(self, message):
        self.message = message

# Continue the definition of the class, adding a method to print
# the class message variable
continue class Foo:
    def second(self):
        print(self.message)

# Create an instance of the class
inst = Foo('Hello World')

# Demo the continued class
inst.second()

# Show that existing syntax still works
for i in range(5):
    if i == 0:
        continue
    print(i)
```
