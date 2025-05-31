## 10.2 Lab – Creating Modules (GitHub Codespaces Version)

### **Introduction**

Creating and using your own Python modules is an essential skill that helps you build reusable, organized, and maintainable code. In this lab, you’ll learn how to create a simple Python module and use it in another script — all within GitHub Codespaces, a cloud-based coding environment.

---

### **Objectives**

By the end of this lab, you will be able to:

* Create a Python module with functions.
* Import and use that module in another Python script.
* Work entirely in GitHub Codespaces without needing local software.

---

### **Lab Steps**

---

### **Step 1: Launch GitHub Codespaces**

1. Go to your GitHub repository for this lab.
2. Click the green **“Code”** button.
3. Under the **“Codespaces”** tab, click **“Create codespace on main”**.
4. Wait for the Codespace to load in the browser-based VS Code environment.

---

### **Step 2: Create the Python Module**

1. In the file explorer on the left, right-click your repository folder and choose **New File**.
2. Name the file: `greetings.py`
3. Add the following code to define the module:

```python
# greetings.py

def say_hello(name):
    print(f"Hello, {name}! Welcome to Python modules.")

def say_goodbye(name):
    print(f"Goodbye, {name}! See you later.")
```

Press **Ctrl + S** to save the file.

---

### **Step 3: Create the Script That Uses the Module**

1. Right-click the file explorer again and choose **New File**.
2. Name the file: `test_greetings.py`
3. Add the following code:

```python
# test_greetings.py

import greetings

# Using the say_hello function from greetings module
greetings.say_hello("Alice")

# Using the say_goodbye function from greetings module
greetings.say_goodbye("Alice")
```

Save the file (**Ctrl + S**).

---

### **Step 4: Run the Script in the Terminal**

1. Open the terminal in Codespaces: go to **Terminal > New Terminal** or press **Ctrl + \`**.
2. Run the script:

```bash
python3 test_greetings.py
```

---

### **Step 5: Expected Output**

The output should be:

```
Hello, Alice! Welcome to Python modules.
Goodbye, Alice! See you later.
```

---

### **Summary**

In this lab, you created a reusable Python module (`greetings.py`) and successfully imported it into another script (`test_greetings.py`) in GitHub Codespaces. You learned the basics of modular programming in Python and gained practical experience using cloud-based tools to build maintainable code.

