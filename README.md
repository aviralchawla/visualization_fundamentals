# Fundamentals of Data Visualization

Basic tutorial for CS undergraduates to understand data visualization and explore relevant Python libraries. This guide will walk you through on how to run all notebooks / code to visualize the data.

## Getting Started

### 0. Prerequisites

Before you begin, make sure you have the following correctly installed on your system:

- **Python**: You must have Python correctly installed (ideally above version 3.9). To make sure that it is correctly installed, open your Terminal / Command Prompt and run the following command:

    ```bash
    python --version
    ```

    If for some reason it is not installed, you can follow the installation [guide](https://realpython.com/installing-python/).

- **Conda** (Optional but recommended): Conda is a package and environment manager that makes it very easy to handle many different projects with their own requirements. I will recommend following the installation [guide](https://docs.conda.io/projects/conda/en/stable/user-guide/getting-started.html). If you do not want it, Python comes with its own built-in virtual environment manager, [venv](https://www.w3schools.com/python/python_virtualenv.asp), so we can use that.

### 1. Getting the Files

To get all the code and data files you can either clone the repository using Git or download it as a ZIP file.

#### Option A: Clone the Repository (Recommended)

Cloning with Git is the best way to stay updated with any changes.
1. Open your terminal (Terminal on Mac/Linux, Command Prompt or Git Bash on Windows).
2. Navigate to the directory where you want to store the project.
3. Run the following command:
```bash
git clone https://github.com/aviralchawla/visualization_fundamentals.git
```

#### Option B: Download the ZIP File

1. On the main GitHub page of this repository, click the green < > Code button.
2. Select Download ZIP.
3. Once downloaded, unzip the folder to your desired location.

### 2. Open the project

After getting the files, you need to navigate into the project directory. Here's how-

**In Terminal**
Open your terminal and use the `cd` command to enter the folder:
```bash
# Replace 'path/to/your/folder' with the actual path
cd path/to/your/folder/visualization_fundamentals
```

**In VS Code** (or any other editor)
1. Open the VS Code application.
2. Go to File > Open Folder...
3. Navigate to and select the `visualization_fundamentals` folder you just cloned or unzipped.
4. Open the built-in terminal in VS Code by going to Terminal > New Terminal. All commands from here on can be run in this VS Code terminal.

### 3. Setting up Virtual Environment

#### Option A: Using `conda`

1. In your terminal (or VS Code terminal), create a new environment. We'll name it `vis_env`:
```bash
conda create --name vis_env python=3.11
```
2. Activate the environment:
```bash
conda activate vis_env
```

#### Option B: Using `venv` (Built-in)

1. In your terminal, create the environment (this creates a folder named .venv):
    - On Mac/Linux:
    ```bash
    python3 -m venv .venv
    ```
    - On Windows:
    ```bash
    python -m venv .venv
    ```
2. Activate the environment:
    - On Mac/Linux:
    ```bash
    source .venv/bin/activate
    ```
    - On Windows:
    ```
    .\.venv\Scripts\activate
    ```

### Install requirements

Once your virtual environment is active, install all the required packages using the requirements.txt file.
```bash
pip install -r requirements.txt
```

### Sanity Check

Now let's make sure everything is correctly installed. Again in command line start Python interpreter:
```bash
python
```
Then:
```python
>> import pandas as pd
>> import matplotlib.pyplot as plt
>> print(pd.__version__, plt.__version__)
```
If there are no `ModuleNotFoundError`, you can exit by typing `exit()`

### Working Notebooks

We also want to make sure you are able to get notebooks working in the editor of your choice. For instance, in VS Code, open `intro.ipynb`, then:
1. Click **Select Kernel** in the top-right corner of the notebook (`intro.ipynb` file)
2. Choose your `vis_env` or `.venv` environment from the list. It might be under "Python Environments".
3. Run all the cells in the notebook.

If you run into any issues, feel free to ask your favorite LLM to help you get it setup. 
