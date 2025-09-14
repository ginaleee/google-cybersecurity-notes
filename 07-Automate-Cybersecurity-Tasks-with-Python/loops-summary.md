Here’s a clean **GitHub-ready summary** of your loops in Python notes:

---

## Loops in Python

Loops allow repeated execution of code based on sequences or conditions. Security analysts use them to process data, automate checks, and control execution.

### 🔁 For Loops

* Best for iterating through a **sequence** (lists, strings, ranges).
* Syntax:

  ```python
  for item in sequence:
      # loop body
  ```
* Examples:

  * Iterating usernames:

    ```python
    for i in ["elarson", "bmoreno", "tshah"]:
        print(i)
    ```
  * Using `range()` for number sequences:

    ```python
    for i in range(5):
        print(i)  # prints 0–4
    ```

### 🔁 While Loops

* Best for iterating **while a condition is True**.
* Syntax:

  ```python
  while condition:
      # loop body
  ```
* Example:

  ```python
  i = 1
  while i < 5:
      print(i)
      i = i + 1
  ```

### ⚡ Controlling Loops

* **break** → exits the loop early.

  ```python
  for asset in ["laptop1", "desktop20", "smartphone03"]:
      if asset == "desktop20":
          break
      print(asset)
  ```
* **continue** → skips current iteration, continues with next.

  ```python
  for asset in ["laptop1", "desktop20", "smartphone03"]:
      if asset == "desktop20":
          continue
      print(asset)
  ```

### ⚠️ Infinite Loops

* A loop without an exit condition runs forever.
* Stop with **CTRL+C** (Linux/Mac) or **CTRL+Z** (Windows).

### ✅ Key Takeaways

* **For loops** → use with sequences (lists, strings, ranges).
* **While loops** → use with conditions that must remain True.
* **break / continue** → control execution flow inside loops.


