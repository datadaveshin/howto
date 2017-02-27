# Print to standard error / stderr
source: http://stackoverflow.com/questions/5574702/how-to-print-to-stderr-in-python
```python
from __future__ import print_function # This line must be at top of file
import sys

def eprint(*args, **kwargs):
    print(*args, file=sys.stderr, **kwargs)
```


