
`numpy` is a library designed to help with working with numbers in Python. It is used most often to do maths with large grids of numbers, which `numpy` calls "arrays".

#### Usage

You can use `numpy` to process the individual pixels in each camera image taken using `picamzero`'s `capture_array` function. For example, you could filter the image to only show the red channel:

```python
from picamzero import Camera
import numpy as np
import PIL

camera = Camera()
image_as_array = camera.capture_array()
red_channel = image_as_array[:, :, 0]
Image.fromarray(red_channel).save("red-channel.jpg")
```

#### Documentation

- [https://numpy.org/doc/stable/user/index.html](https://numpy.org/doc/stable/user/index.html)
