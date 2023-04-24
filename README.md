# Outlier Detection

This is a Python library for outlier detection. It provides a set of algorithms for detecting outliers in datasets, including statistical methods, distance-based methods, and machine learning-based methods. 

## Installation

To install the package, clone the repository and run the following command in the project directory:

```
pip install -r requirements.txt
```

## Usage

To use the outlier detection algorithms in this package, import the `OutlierDetection` class from the `outlier_detection` module:

```python
from outlier_detection import OutlierDetection
```

Then, create an instance of the `OutlierDetection` class and call one of the available methods, passing in your data as a NumPy array or Pandas DataFrame:

```python
import numpy as np
import pandas as pd

data = np.array([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]])
od = OutlierDetection()
results = od.univariate_zscore(data)
print(results)
```

## Algorithms

This package includes the following algorithms for outlier detection:

* Univariate Z-Score
* Multivariate Z-Score
* Mahalanobis Distance
* Local Outlier Factor
* Isolation Forest

Each method returns an array of scores indicating the degree of outlierliness of each data point. The higher the score, the more likely the point is an outlier.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
