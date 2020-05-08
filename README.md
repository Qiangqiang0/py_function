# py_function

## 1. read file from start to stop

```python
def read_data(fname,stop,start=0):
  out = []
  from itertools import islice
  with open(fname) as f:
    for line in islice(f,start=start,stop=stop):
    out.append(line)
  return out
      
```
