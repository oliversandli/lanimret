# lanimret

*lanimret* is a simple, clear module giving full terminal control on \*nix systems. The detested *curses* library will never have to show its face in your code again.

## Dependencies

*lanimret* is written in Python v3.7 with only modules from the standard library.

## Installation

### pip

```bash
pip install lanimret
```

### Github

```bash
git clone https://github.com/oliversandli/lanimret.git
```

## Examples

```python
from lanimret import Color as co

# print blue text and then blue text with a red background

print(f"{co.fg.blue}This is blue text! {co.bg.red}And with a red background.{co.reset}")
```

```python
import time
from lanimret import Cursor

# a simple progress indicator

cur = Cursor()

for i in range(101)
    print(f"{i}%", end="")
    time.sleep(0.05)
    cur.clear_line(2)
```
