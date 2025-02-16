# Installation Guide

This document provides a comprehensive guide to setting up the required environment for exploring and running the exercises provided in the **Python for Engineers** repository. Please ensure you follow the steps precisely to avoid any issues during installation.

## Prerequisites

Before proceeding with the installation, ensure that your system meets the following prerequisites:

1. **Python Installation**

   - Python version 3.8 or higher is required.
   - To verify if Python is installed, open a terminal or command prompt and execute:

     ```bash
     python --version
     ```

     or

     ```bash
     python3 --version
     ```

   - If Python is not installed, download the latest version from the official Python website:
     [https://www.python.org/downloads/](https://www.python.org/downloads/).

2. **Jupyter Notebook**

   - Jupyter Notebook is the platform used to run and interact with the exercises.
   - It is recommended to install Jupyter via a Python package manager such as `pip` or within a virtual environment.

3. **Package Manager (pip)**
   - Ensure that `pip`, the Python package manager, is installed. To verify, execute:

     ```bash
     pip --version
     ```

   - If `pip` is not available, refer to the official guide to install it:
     [https://pip.pypa.io/en/stable/installation/](https://pip.pypa.io/en/stable/installation/).

## Installation Steps

### 1. Clone the Repository

Begin by cloning the repository to your local machine. Open a terminal or command prompt and execute the following command:

```bash
git clone https://github.com/david-palma/python-for-engineers.git
```

Navigate to the repository directory:

```bash
cd python-for-engineers
```

### 2. Create a Virtual Environment (optional)

It is strongly recommended to use a virtual environment to manage dependencies independently. Execute the following commands to create and activate a virtual environment:

#### **Windows**

1. Create the virtual environment:

   ```bash
   python -m venv venv
   ```

2. Activate the virtual environment:

   ```bash
   venv\Scripts\activate
   ```

#### **Unix-like**

1. Create the virtual environment:

   ```bash
   python3 -m venv venv
   ```

2. Activate the virtual environment:

   ```bash
   source venv/bin/activate
   ```

Once the virtual environment is activated, the terminal or command prompt should display a prefix indicating the environment is active (e.g., `venv`).

#### Deactivating the Virtual Environment

When finished working, deactivate the virtual environment by running:

```bash
deactivate
```

### 3. Install Required Dependencies

The repository includes a `requirements.txt` file that specifies all the Python libraries and packages required to run the exercises. Install these dependencies using the following steps:

1. Ensure that you are in the root directory of the repository.

   ```bash
   cd python-for-engineers
   ```

2. If you have activated a virtual environment (optional but recommended), ensure it is active. Refer to Step 2 for details on activating the virtual environment.
3. Install the dependencies listed in the `requirements.txt` file using pip:

   ```bash
   pip install -r requirements.txt
   ```

   This command will install libraries such as:

   - numpy (for numerical computations),
   - matplotlib (for visualisations),
   - pandas (for data manipulation),
   - scipy (for advanced computations),
   - Additional libraries required for specific exercises.

### 4. Verify the Installation

To ensure all dependencies are correctly installed, execute the following command to list installed packages:

```bash
pip list
```

Alternatively, test the setup by running a Jupyter Notebook.

## Running the Exercises

### 1. Launch Jupyter Notebook

Start the Jupyter Notebook server by executing:

```bash
jupyter notebook
```

A browser window should open automatically, displaying the Jupyter interface. Navigate to the `case-studies/` folder and select a exercise notebook (e.g., `01-gear-wear-analysis.ipynb`) to open.

### 2. Execute the Notebook

Once the notebook opens:

- Read the introductory section to understand the context of the exercise.
- Execute the cells sequentially to reproduce the results and visualisations.

## Running Exercises in Visual Studio Code (Alternative)

If you prefer using **Visual Studio Code (VS Code)** to explore and run the exercises, follow the steps below to set up and run the notebooks effectively.

#### 1. Install Visual Studio Code

- Download and install VS Code from the official website:
  [https://code.visualstudio.com/](https://code.visualstudio.com/).

#### 2. Install Required Extensions

To enable support for Python and Jupyter Notebooks, install the following extensions:

- **Python Extension** (by Microsoft)
- **Jupyter Extension** (by Microsoft)

To install these extensions:

1. Open VS Code.
2. Navigate to the Extensions view by clicking the Extensions icon in the Activity Bar on the side of the window or pressing `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (macOS).
3. Search for and install the following:
   - _Python_
   - _Jupyter_

#### 3. Open the Repository in VS Code

1. Open VS Code and select **File > Open Folder...** to open the `python-for-engineers` repository directory.
2. Alternatively, you can open the terminal in the repository directory and execute:

   ```bash
   code .
   ```

#### 4. Open and Run a Exercise

1. In the VS Code Explorer (left-hand side), navigate to the `case-studies/` folder.
2. Open the desired Jupyter Notebook file (e.g., `01-gear-wear-analysis.ipynb`).
3. If prompted, select the Python interpreter associated with your virtual environment.
   - You will see a notification at the top-right of the VS Code interface to select the interpreter.
4. Run the cells sequentially by clicking the Run button (►) at the top of each cell or using the toolbar controls provided for notebooks.

#### 5. Debugging and Troubleshooting

To debug Python scripts or cells in a Jupyter Notebook:

- Add breakpoints in the code by clicking to the left of the line numbers.
- Use the Run and Debug feature in VS Code, accessible from the Activity Bar on the side.

## Troubleshooting

While setting up and running the exercises, you may encounter some issues. Below are common problems and their solutions to help you resolve them.

### 1. Jupyter Notebook Not Launching

**Problem**: Running `jupyter notebook` results in an error or no action.

**Solution**:

- Ensure that you have installed Jupyter in your environment by running:

  ```bash
  pip install notebook
  ```

- If you are using a virtual environment, make sure it is activated before running the command.
- Try upgrading Jupyter with:

  ```bash
  pip install --upgrade notebook
  ```

### 2. Missing Dependencies or ModuleNotFoundError

**Problem**: When running a notebook, you encounter a `ModuleNotFoundError` for a missing package.

**Solution**:

- Ensure all dependencies are installed by running:

  ```bash
  pip install -r requirements.txt
  ```

- Verify the correct virtual environment is activated (if using one).
- Check the specific module mentioned in the error and install it manually:

  ```bash
  pip install <module_name>
  ```

### 3. Issues with Visual Studio Code Extensions

**Problem**: The Jupyter Notebook does not run as expected in Visual Studio Code.

**Solution**:

- Ensure that both the **Python** and **Jupyter** extensions are installed in VS Code, as described in the instructions provided in section [Running Exercises in Visual Studio Code](#running-case-studies-in-visual-studio-code-alternative).
- If notebooks do not open correctly, try reloading the window:
    - Click on **View > Command Palette**, then type and select **Reload Window**.
- Ensure that the correct Python interpreter is selected. You should see a notification at the top-right of the VS Code interface to choose the interpreter. Select the one associated with your virtual environment (if using one).

### 4. Kernel or Runtime Errors in Jupyter Notebooks

**Problem**: You receive an error like "Kernel Restarting" or similar when executing cells in Jupyter.

**Solution**:

- This often occurs when dependencies are not installed correctly. Ensure all required packages are installed with:

  ```bash
  pip install -r requirements.txt
  ```

- If using a virtual environment, ensure it is active.
- Restart the Jupyter kernel by selecting **Kernel > Restart** in the notebook interface.

### 5. Virtual Environment Issues

**Problem**: The virtual environment is not activating properly.

**Solution**:

- Ensure you are in the correct directory when trying to activate the virtual environment.
- On **Windows**, use:

  ```bash
  venv\Scripts\activate
  ```

- On **Unix-like** systems, use:

  ```bash
  source venv/bin/activate
  ```

  If the environment still fails to activate, recreate it by deleting the `venv/` folder and running:
- On **Windows**

  ```bash
  python -m venv venv
  ```

- On **Unix-like** systems

  ```bash
  python3 -m venv venv
  ```

### 6. Dependency Version Conflicts

**Problem**: Conflicting versions of dependencies cause errors or unexpected behaviour.

**Solution**:

- Check the versions of installed dependencies using:

  ```bash
  pip list
  ```

- If a conflict exists, try upgrading or downgrading the specific package to match the required version:

  ```bash
  pip install <module_name>==<desired_version>
  ```

### 7. Visualisation Not Displaying Correctly

**Problem**: Plots or graphs do not render in the notebook or show as blank figures.

**Solution**:

- Ensure that you have the necessary plotting libraries installed, such as `matplotlib` or `seaborn`.
- In Jupyter, ensure you include the following magic command at the beginning of the notebook to enable inline plotting:

  ```python
  %matplotlib inline
  ```

- Check that the notebook cells are being executed in the correct order, as plots may rely on variables created in previous cells.

### 8. Performance Issues

**Problem**: The exercises run slowly or consume excessive resources.

**Solution**:

- Ensure that your environment meets the system requirements for running the exercises, especially for more complex simulations.
- Close other applications to free up system resources.
- For large computations, consider breaking down the problem into smaller chunks or using more efficient algorithms.

### General Installation Issues

**Problem**: If you face any other installation or setup issues not addressed here, consider the following steps:

**Solution**:

- Ensure that Python is correctly installed by running:

```bash
python --version
```

- Ensure that `pip` is up-to-date by running:

  ```bash
  python -m pip install --upgrade pip
  ```

- Review any error messages carefully for additional clues or missing dependencies.
