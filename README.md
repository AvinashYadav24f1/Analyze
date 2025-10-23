# Data Analysis and Automation Workflow

This project demonstrates a robust and automated workflow for data analysis, covering data preparation, script execution, code quality enforcement, and automated publishing of results using GitHub Actions and GitHub Pages.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Technical Implementation Details](#technical-implementation-details)
- [Live Demo](#live-demo)
- [License](#license)

## Project Overview

The core objective of this project is to process tabular data, specifically converting an Excel file (`data.xlsx`) into a CSV format (`data.csv`), executing a Python script (`execute.py`) to perform analysis, and then automating the entire process, including code quality checks and result publishing. The `execute.py` script was also reviewed and fixed to ensure correct operation and adherence to specified Python and Pandas versions.

## Features

*   **Data Transformation**: Converts `data.xlsx` to `data.csv` for consistent and efficient data processing.
*   **Python Script Execution**: Runs the `execute.py` script, which performs data analysis and generates a `result.json` output.
*   **Code Quality Assurance**: Integrates `ruff` for fast linting and formatting of Python code, ensuring high code quality standards and maintainability.
*   **Automated Workflow (CI/CD)**: Utilizes GitHub Actions to automate the entire process on every push to the repository, including:
    *   Running `ruff` checks.
    *   Executing `execute.py` to generate `result.json`.
    *   Publishing `result.json` as a static asset.
*   **Live Output Publishing**: Publishes the generated `result.json` to GitHub Pages, making the analysis results publicly accessible and easy to share.
*   **Environment Consistency**: Ensures compatibility and execution on Python 3.11+ with Pandas 2.3, leveraging modern language features and robust data handling capabilities.

## Setup Instructions

To set up and run this project locally, follow these steps:

### Prerequisites

*   Git
*   Python 3.11+

### Local Setup

1.  **Clone the repository:**