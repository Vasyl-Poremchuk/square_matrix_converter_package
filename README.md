## Square Matrix Converter Package

### Description

A package that converts a square matrix to a one-dimensional list.

            +-----+-----+-----+-----+
            |  10 |  20 |  30 |  40 |
            +-----+-----+-----+-----+
            |  50 |  60 |  70 |  80 |
            +-----+-----+-----+-----+    ----->    [160, 150, 140, 130, 90, 50, 10, 20, 30, 40, 80, 120, 110, 100, 60, 70]
            |  90 | 100 | 110 | 120 |
            +-----+-----+-----+-----+
            | 130 | 140 | 150 | 160 |
            +-----+-----+-----+-----+
                                    

### Example of How To Use

Install the package using the command below:

```python
pip install square-matrix-converter
```

Use the code below:

```python
import asyncio

from square_matrix_converter import parse_matrix


URL = "https://raw.githubusercontent.com/koury/pymx/main/source.txt"

loop = asyncio.new_event_loop()
asyncio.set_event_loop(loop)
one_dimensional_list = loop.run_until_complete(parse_matrix(URL))

print(one_dimensional_list)
```
