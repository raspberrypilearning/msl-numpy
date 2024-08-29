
`numpy` is a general-purpose array processing library designed to efficiently manipulate large multidimensional arrays (e.g. matrices) of arbitrary records without sacrificing too much speed for small multidimensional arrays.

#### Usage

`numpy` is particularly handy for manipulating raw camera output:

```python
from picamzero import Camera
import numpy as np

camera = Camera()
image_as_array = camera.capture_array()
red_channel = image_as_array[:, :, 0]
```

#### Documentation

- [https://numpy.org/doc/stable/user/index.html](https://numpy.org/doc/stable/user/index.html)
