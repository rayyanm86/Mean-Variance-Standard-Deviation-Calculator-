## 📊 Mean-Variance-Standard Deviation Calculator
This project is part of freeCodeCamp's Data Analysis with Python certification. It implements a function in Python that uses NumPy to compute key statistical properties of a 3×3 matrix.

---

### ✅ Features

The `calculate()` function performs the following operations on a 3×3 matrix derived from a user-provided list of 9 numbers:

* **Mean**
* **Variance**
* **Standard Deviation**
* **Maximum**
* **Minimum**
* **Sum**

These statistics are calculated:

* Along **axis 0** (columns),
* Along **axis 1** (rows),
* And for the **flattened matrix**.

---

### 📁 File Structure

```
boilerplate-mean-variance-standard-deviation-calculator/
│
├── mean_var_std.py         # Main module containing the calculate() function
├── main.py                 # Used to manually run and test the function
├── README.md               # This file
```

---

### 🚀 Usage

1. Clone the repository or open it in [Replit](https://replit.com/) / Gitpod.

2. Add the following test to `main.py`:

```python
from mean_var_std import calculate
print(calculate([0,1,2,3,4,5,6,7,8]))
```

3. Run the file:

```bash
python3 main.py
```

---

### 🔍 Example Output

```python
calculate([0,1,2,3,4,5,6,7,8])
```

```json
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.666..., 0.666..., 0.666...], 6.666...],
  'standard deviation': [[2.449..., 2.449..., 2.449...], [0.816..., 0.816..., 0.816...], 2.581...],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

---

### ⚠️ Error Handling

If the input list does not contain exactly 9 elements, the function raises:

```python
ValueError: List must contain nine numbers.
```

---

### 🧪 Running Unit Tests

Run the included unit tests with:

```bash
python3 -m unittest test_module.py
```

---

### 🛠️ Built With

* Python 3
* NumPy

---

### 📜 License

This project is licensed under the [MIT License](LICENSE).
