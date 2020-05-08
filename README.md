# py_function

## 1. read file from start to stop

```python
def read_data(fname,stop,start=0):
  assert (stop > start), "stop should larger than start"
  out = []
  from itertools import islice
  with open(fname) as f:
    if start == 0 :
    
      for line in islice(f,stop):
        out.append(line)
    else:
      for line in islice(f,start,stop):
        out.append(line)
  return out
      
```
