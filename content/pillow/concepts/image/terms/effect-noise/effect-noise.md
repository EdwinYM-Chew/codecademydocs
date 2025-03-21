---
title: "effect_noise"
summary: "Applies random noise to an image, creating a textured effect."
---

## Overview

The `.effect_noise()` method in the **Pillow (PIL) library** applies a random noise pattern to an image. This effect is useful for generating textures, artistic effects, or simulating natural noise in digital images.

## Syntax

```python
Image.effect_noise(size, sigma)
```

### Parameters

| Parameter | Type  | Description |
|-----------|-------|-------------|
| `size`    | `int` | The size of the noise pattern. A larger value results in a more spread-out noise texture. |
| `sigma`   | `float` | The standard deviation of the noise distribution. Higher values increase the intensity of the noise. |

## Example

```python
from PIL import Image

# Create a blank grayscale image
img = Image.new("L", (300, 300), "white")

# Apply effect_noise
noisy_img = img.effect_noise(100, 8.0)

# Show and save the result
noisy_img.show()
noisy_img.save("effect_noise_example.png")
```

### Output
The above code generates a **grayscale image** with a noise pattern, creating a textured effect. The result can be used for synthetic textures or artistic modifications.

## Use Cases
- Creating artificial textures for graphic design.
- Simulating real-world noise effects in images.
- Generating random patterns for image processing applications.

## Additional Resources
- [Pillow Documentation](https://pillow.readthedocs.io/)
- [Image Module in Pillow](https://pillow.readthedocs.io/en/stable/reference/Image.html)

---



