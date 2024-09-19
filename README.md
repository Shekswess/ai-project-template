# ai-project-template

Welcome to the AI Project Template repository. This template is designed to streamline the development and deployment of AI/ML/MLOps/LLMOps projects. It provides a comprehensive setup for experiment tracking, model versioning, monitoring, tracing, and efficient project management, ensuring that all critical aspects of an AI project are covered. Below is a detailed breakdown of the repository structure, tools, and configuration files included.

## Included Features
- **GitHub Actions**: CI/CD workflows examples for testing code, it can be extended to deploy models, run experiments, and more.
- **Config Directory**: Centralized configuration files for the project.
- **Data Directory**: Organized folders for raw, processed, and database data.
- **IaC Directory**: Infrastructure as Code (IaC) scripts for cloud deployment.
- **Notebooks Directory**: Jupyter notebooks for exploratory data analysis and experiments.
- **Results Directory**: Folder to store the results of experiments and models.
- **Source Code Directory**: Organized source code for models, pipelines, utilities, and constants.
- **Tests Directory**: Unit and integration tests for the project.
- **.env File**: Environment variables file for sensitive information.
- **.gitignore File**: Git ignore file for ignoring unnecessary files and directories.
- **pre-commit Configuration**: Pre-commit configuration for general checks, type checking, linting and formatting, python updates, secret detection, licence insertion, and more.
- **Docker Compose**: Docker Compose setup for MLflow, Langfuse, and databases + storage for them.
- **Conda Environment**: Environment configuration file for managing Python environments - currently using Python 3.11.
- **Pyproject.toml File**: Configuration for ruff formatter and linter
- **Requirements.txt File**: Python dependencies for the project.


## Repository Structure
```bash
.
├── config                # Configuration files for your project
│   └── config.yaml
├── data                  # Folder to store raw and processed data
│   ├── database          # Databases or local data storage
│   ├── processed         # Preprocessed/cleaned data
│   └── raw               # Raw data inputs
├── iac                   # Infrastructure as Code (IaC) scripts for cloud deployment
├── docker-compose.yaml   # Docker Compose setup for MLflow, Langfuse, and related services
├── environment.yaml      # Conda environment configuration file
├── notebooks             # Jupyter notebooks for exploratory data analysis, experiments
│   └── 00_example.ipynb
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
