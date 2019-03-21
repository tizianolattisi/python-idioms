Creating DTOs (POJOs/POCOs)
```python
from collections import namedtuple
Customer = namedtuple("Customer", "name email")
customer = Customer("John", "john@domain.com")
```


Default values for function parameters
```python
def foo(a, b = ""):
    pass
```

Filtering a list
```python
positives = [n for n in l if n>0]
```
or

```python
positives = list(filter(lambda n: n>0, l))
```

String Interpolation
```python
print("Name {name}".format(name="..."))
```

Instance Checks
```python
def test(x):
    if isinstance(x, A):
        pass
    elif isinstance(x, B):
        pass
```

Traversing a map/list of pairs
```python
for k, v in zip(my_map.keys(), my_map.values()):
     print ("{k} -> {v}".format(k=k, v=v))
```

Using ranges
```python
for i in range(1, 101): # closed range: includes 100
    pass

for i in range(1, 100): # half-open range: does not include 100
    pass

for i in [x for x in range(2,11) if not x%2]:
    pass

for i in reversed(range(1, 11)):
    pass

if x in range(1, 11):
    pass
```

Read-only list
```python
l = ("a", "b", "c") # a tuple is immutable
```

Read-only map
```python
# to implements with collections.Mapping?
```

Accessing a map
```python
print(my_map["key"])
my_map["key"] = value
```

Lazy property
```python
# ?
```

Extension FUnctions
```python
MyClass.spaceToCamelCase = lambda self, s: s # TODO
```

Creating a singleton
```python
# with a instance reference static field?
```

If not null shorthand
```python
files and print(len(files))
```

If not null and else shorthand
```python
print (files and len(files) or "empty")
```

Executing a statement if null
```python
email = values["email"] or print("empty")
```

Get first item of a possibly empty collection
```python
main_email = emails and emails[0] or ""
```
