---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.19.5
kernelspec:
  name: python3
  display_name: Python 3 (ipykernel)
  language: python
---

# Code

```{code-cell} ipython3
import numpy as np

# TODO: fill in your chosen dart count and a seed of your own
np.random.seed(42)
n_darts = 100

x = np.random.uniform(-1, 1, n_darts)
y = np.random.uniform(-1, 1, n_darts)
inside_circle = (x**2 + y**2) <= 1

pi_estimate = 4 * inside_circle.sum() / n_darts
print(f"Darts thrown: {n_darts:,}")
print(f"Estimated pi: {pi_estimate:.5f}")
```

```{warning} alert!
warning
```

+++

# Results

+++

```{figure} images/throwingdarts.png
:name: throwing darts
figure
```

```{code-cell} ipython3

```
