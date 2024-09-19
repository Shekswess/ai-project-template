# ai-project-template

[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)

Welcome to the **AI Project Template** repository! This template is designed to **streamline the development** and **deployment** of AI/ML/MLOps/LLMOps projects. It provides a comprehensive setup for experiment tracking, model versioning, monitoring, tracing, and efficient project management, ensuring that all critical aspects of an AI project are covered.

## 🚀 Features Included

- **[GitHub Actions](https://docs.github.com/en/actions)**: CI/CD workflows for testing code, deploying models, running experiments, and more.
- **Config Directory**: Centralized configuration files for the project.
- **Data Directory**: Structured data management (raw, processed, and database data).
- **IaC Directory**: Infrastructure as Code (IaC) scripts for cloud deployment.
- **Notebooks Directory**: Jupyter notebooks for data analysis and experiments.
- **Results Directory**: Store experiment results, logs, and models.
- **Source Code Directory**: Modularized source code for models, pipelines, utilities.
- **Tests Directory**: Unit and integration tests using `pytest`.
- **[pre-commit](https://pre-commit.com/)**: Configuration for linting, type checking, and secret detection.
- **[Docker Compose](https://docs.docker.com/compose/)**: Setup for services like MLflow, Langfuse, databases, and storage.
- **[Conda Environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)**: Python 3.11 environment configuration.
- **[Pyproject.toml](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/)**: Config for ruff linter, formatter, type checking, and testing.
- **[Requirements.txt](https://pip.pypa.io/en/stable/user_guide/#requirements-files)**: Python dependencies file.


> [!NOTE]
> Not every element from this template is required for every project. Please adjust the repository structure and configuration files to fit your project's needs.

---

## 📁 Detailed Directory Breakdown

- **`/config`**: Store all configuration files needed for your project.
  - Example: `config.yaml` can be used for setting up hyperparameters, API keys, or other environment variables.

- **`/data`**: Structured data folders for different stages of the project.
  - `raw/`: Raw data straight from the source.
  - `processed/`: Cleaned and preprocessed data ready for use in models.
  - `database/`: Database files if using local storage solutions.

- **`/iac`**: Infrastructure as Code scripts for automating cloud deployments (e.g., AWS CloudFormation, Terraform).

- **`/notebooks`**: Jupyter notebooks for performing Exploratory Data Analysis (EDA), experimenting with models, and reporting.
  - Example: `00_example.ipynb` shows how a notebook looks in the project.

- **`/src`**: Main source code for your project.
  - `/models/`: Machine learning models (e.g., neural networks, decision trees) scripts, classes, and functions.
  - `/pipelines/`: Data and model pipelines.
  - `/constants/`: Store project-wide constants (e.g., file paths, API endpoints).
  - `/utils/`: Utility functions and helpers (e.g., data loaders, preprocessing functions).

- **`/tests`**: Unit and integration tests.

---

## ⚙️ Configuration Files

- **`docker-compose.yaml`**: A Docker Compose configuration to spin up services such as [MLflow](https://mlflow.org/), [Langfuse](https://www.langfuse.com/), databases, and any additional tools.

- **`environment.yaml`**: [Conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) file to manage Python dependencies.
  - Python version: **3.11**

- **`.env`**: Store environment variables like API keys, database credentials, and sensitive information.

- **`.gitignore`**: Standard [`.gitignore`](https://git-scm.com/docs/gitignore) file to exclude unnecessary files (e.g., environment files, data files).

---

## 🛠️ How to Use

### 1. **Clone the Repository**
```bash
git clone https://github.com/username/ai-project-template.git
cd ai-project-template
```

### 2. Set Up Conda Environment
```bash
conda env create -f environment.yaml
conda activate ai-project
```

### 3. Install Python Dependencies
```bash
pip install -r requirements.txt
```

### 4. Start Docker Compose Services (Optional)
```bash
docker-compose up -d
```

---

## 🗂️ Repository Structure
```bash
.
├── config                # Configuration files for your project
│   └── config.yaml       # Example configuration file
├── data                  # Folder to store raw and processed data
│   ├── database          # Databases or local data storage
│   ├── processed         # Preprocessed/cleaned data
│   └── raw               # Raw data inputs
├── iac                   # Infrastructure as Code (IaC) scripts for cloud deployment
├── docker-compose.yaml   # Docker Compose setup for MLflow, Langfuse, and related services
├── environment.yaml      # Conda environment configuration file
├── notebooks             # Jupyter notebooks for exploratory data analysis, experiments
│   └── 00_example.ipynb  # Example notebook
├── pyproject.toml        # Configuration for formatting, linting, type-checking, and testing
├── README.md             # Documentation for the project (you're reading it!)
├── requirements.txt      # Python dependencies for your project
├── results               # Folder to store the results of experiments and models
├── src                   # Source code of your project
│   ├── constants         # Constants used in the project
│   ├── execution.py      # Main execution script
│   ├── models            # Machine learning model scripts
│   ├── pipelines         # ML pipelines for preprocessing and modeling
│   └── utils             # Utility functions
└── tests                 # Unit and integration tests
    └── test.py           # Example test file using pytest
```

---

## 📋 Contributing
Feel free to contribute to this project by submitting a pull request.
