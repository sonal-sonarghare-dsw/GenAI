# 🧪 Python Environments Guide

A **Python environment** is an isolated workspace that allows you to manage your Python version and project-specific dependencies. This is crucial for ensuring consistency and avoiding conflicts across projects.
- A specific **Python interpreter version** (e.g., Python 3.8, 3.11)
- A custom set of **installed packages and dependencies**

## Types of Python Environments

### 1. Global Environment: 
The default Python installation on your system.

---

### 2. Virtual Environments (venv)
Isolated environments that allow you to manage dependencies for specific projects. 

#### 🔹 Create a virtual environment:
```bash
python -m venv myenv
```

#### 🔹 Create with a specific Python version:
```bash
py -3.10 -m venv myenv310
```

#### 🔹 Activate the environment (Windows):
```bash
myenv\Scripts\activate
```

#### 🔹 Deactivate the environment:
```bash
deactivate
```

---

### 3. Conda Environments (via Anaconda)
A powerful environment manager, especially useful for data science and scientific computing.

#### ✅ Create a Conda environment:
```bash
conda create -n myenv python=3.9
```

#### ✅ Activate environment:
```bash
conda activate myenv
```

#### ✅ Install packages:
```bash
conda install numpy pandas matplotlib
```

#### ✅ Deactivate environment:
```bash
conda deactivate
```

#### ❌ Remove the environment:
```bash
conda remove -n myenv --all
```

#### 📋 List all Conda environments:
```bash
conda env list
```