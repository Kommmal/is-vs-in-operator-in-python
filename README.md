
# 📝 Assignment 3: Python Operators – `is` vs `in`

In this assignment, I researched and practiced the difference between the `is` and `in` operators in Python. Both are comparison operators but are used for very different purposes.

---

## 🔹 `is` Operator – Identity Comparison

The `is` operator checks whether two variables point to the **same object in memory**. It doesn’t compare the values or contents, just whether both variables refer to the same thing.

### ✅ Example 1:
```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)  # True – because a and b are the same object
print(a is c)  # False – c has the same content but is a different object
```

### ✅ Example 2:
```python
x = 100
y = 100
print(x is y)  # True – small integers are cached in Python
```

In short, `is` is used when we want to check if two variables point to the **same memory location**.

---

## 🔹 `in` Operator – Membership Test

The `in` operator is used to check whether a **value exists inside a collection or sequence**, such as a list, string, tuple, set, or dictionary.

### ✅ Example 1:
```python
fruits = ['apple', 'banana', 'cherry']
print('banana' in fruits)  # True – 'banana' is present in the list
```

### ✅ Example 2:
```python
text = "hello world"
print('h' in text)    # True
print('z' in text)    # False
```

The `in` operator is helpful for searching within iterables like lists or strings.

---

## 🔍 Summary Table

| Operator | Used For               | What it Does                                | Example               | Output      |
|----------|------------------------|---------------------------------------------|------------------------|-------------|
| `is`     | Identity Comparison     | Checks if two variables point to same object | `a is b`              | True / False |
| `in`     | Membership Test         | Checks if a value exists in a collection     | `'a' in 'apple'`      | True / False |

---

## ✅ What I Learned

- `is` is used to check if two variables are actually **the same object in memory**.
- `in` is used to check if something **exists within a collection or sequence**.
- Although both are comparison operators, they are used in very different situations.
- I also learned how Python internally handles small integers and objects in memory using the `is` operator.

---

This assignment helped me understand these concepts better by writing code and testing different scenarios myself. It’s clearer to me now when to use `is` and when to use `in`.
