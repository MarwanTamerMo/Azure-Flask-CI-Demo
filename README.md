# 🚀 Flask & Azure Pipelines CI Demo 🚀

![Azure Pipelines CI Status](https://dev.azure.com/YOUR_ORG_NAME/demo-project/_apis/build/status/flask-demo?branchName=main)
![Docker Build](https://img.shields.io/badge/Docker-Build%20%26%20Push-blue?style=for-the-badge&logo=docker)
![Python Version](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python)

This project demonstrates a complete, automated CI (Continuous Integration) pipeline for a simple Flask web application using **Azure Pipelines**. The pipeline automatically runs unit tests, builds a Docker image, and pushes it to Docker Hub, all triggered by a push to the main branch.

The entire process runs on a **self-hosted agent**, showcasing how to integrate your own infrastructure with Azure DevOps.

---

### 🛠️ Tech Stack

-   **Framework**: Flask
-   **Testing**: Pytest
-   **Containerization**: Docker
-   **CI/CD**: Azure Pipelines
-   **Hosting**: Self-Hosted Agent

---

### 🏁 Getting Started

To get a copy of this project up and running on your local machine, follow these steps.

#### Prerequisites

Make sure you have the following software installed:
* [Python 3.10+](https://www.python.org/downloads/)
* [Docker Desktop](https://www.docker.com/products/docker-desktop/)
* [Git](https://git-scm.com/downloads/)

#### Installation

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd flask-demo
    ```

2.  **Create and activate a Python virtual environment:**
    ```bash
    # For macOS/Linux
    python3 -m venv venv
    source venv/bin/activate

    # For Windows
    python -m venv venv
    .\venv\Scripts\activate
    ```

3.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Flask application locally:**
    ```bash
    flask run
    ```
    The application will be available at `http://127.0.0.1:5000`.

---

### 🔬 Build and Test

This project is configured for automated testing and containerization.

#### Running Tests

To run the unit tests locally, execute the following command from the project's root directory:
```bash
pytest