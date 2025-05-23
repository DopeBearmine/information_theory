# Introduction
A rust library for calculating Information Theoretics

# Examples
```
python3.11 -m venv .venv
source .venv/bin/activate
pip install maturin numpy
maturin develop
```

```
python
>>> from information_theory import entropy
>>> import numpy as np
>>>
>>> data = np.random.normal(0,1,10000)
>>> result = entropy(data, "kde", None)
# entropy(data, data_type, bin_size)
#  - data: list of data points
#  - data_type: "data" (calculate directly) or "kde" (sample after calculating Kernel Density Estimation)
#  - bin_size: float, width of bins to calculate probabilities, defaults to Scotts rule
```
