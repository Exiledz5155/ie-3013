Here’s a similar README adapted for setting up **Julia** and **Python** environments in your repository:

---

# IE-3013 

This repository is a boilerplate/template for classwork in CSCI 4521, now featuring both **Julia** and **Python** setups!

## Setup Instructions

### 1. **Install Python 3.12 or newer**:

- Download and install Python from the [official Python website](https://www.python.org/downloads/).
- **Make sure** to check the option to **'Add Python to PATH'** during installation.

### 2. **Install Julia**:

- Download and install Julia from the [official Julia website](https://julialang.org/downloads/).
- Once installed, you can verify the installation by typing `julia` in your terminal or command prompt.

### 3. **Clone the Repository and Set Up Python Virtual Environment**:

- Skipping the cloning step here; just lock in

- **Create a Python virtual environment**:

  ```bash
  python -m venv venv
  ```

### 4. **Activate the Python Virtual Environment**:

- **For Windows**:

  ```bash
  .\venv\Scripts\activate
  ```

- **For Linux/macOS**:
  ```bash
  source venv/bin/activate
  ```

Remember to activate the virtual environment each time you open a new terminal session.

### 5. **Install Python Dependencies**:

```bash
pip install -r requirements.txt
```

### 6. **Set Up Julia Environment**:

- Navigate to your project directory with cd (this repo) in a separate terminal.
- Start **Julia** by typing `julia` in the terminal.
- Activate the project environment:
  ```julia
  ] activate .
  ```
- **Install Julia dependencies** specified in `Project.toml`:

  ```julia
  ] instantiate
  ```

  This will automatically install all the Julia packages listed in the `Project.toml` and `Manifest.toml`.

  Note: you don't need the "]" if you are already used it once.

## Jupyter Notebook

Again, in a separate terminal:

- To start the Jupyter Notebook:
  ```bash
  jupyter notebook
  ```

You should be able to select both Python and Julia kernals as shown below:

![image](https://github.com/user-attachments/assets/319547b6-dd04-414f-8d12-9b0f2b446130)


### Saving as PDF

File -> Save and Export Notebook as -> HTML

![image](https://github.com/user-attachments/assets/20ddb9ca-750e-4e6c-90d4-e4ceea31903c)

Then, open the HTML file and right-click -> Print -> Save as PDF.

![image](https://github.com/user-attachments/assets/d722d11e-1bf5-4864-8981-59ba51ef7c90)

## Lints and formatters

This section isn't needed, nor completely supported by this repo.

### For Python:

- If using **VSCode**, I recommend installing the extensions for **Flake8** and **mypy**.
- **Prettier** is recommended as the code formatted (might conflict with the Julia one idk).

### For Julia:

You can also install the **JuliaFormatter** extension for **VSCode**.

## Cloning vs. Forking

If you plan to push your code to GitHub, it’s recommended you **fork** this repository and make it private.

For saving things locally, **cloning** the repository is sufficient.
