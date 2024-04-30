# Web Application CI/CD Pipeline

This repository contains a basic web application along with a CI/CD pipeline implemented using GitHub Actions.

## Source Code

- The source code for the web application can be found in `app.py`.
- Unit tests for the application are located in `test_app.py`.
- Python dependencies are listed in `requirements.txt`.

## GitHub Actions Workflow

- The workflow configuration for CI/CD pipeline is defined in `.github/workflows/main.yml`.
- The workflow triggers on every push to the `main` branch.
- It runs tests, and if successful, deploys the application to Railway.

## Running the Application and Pipeline

To run the application locally:

1. Install Python 3.10.
2. Clone this repository.
3. Navigate to the repository directory.
4. Install dependencies: `pip install -r requirements.txt`.
5. Run the application: `python app.py`.
6. Access the application at `http://localhost:5000`.

To run the pipeline:

1. Fork this repository.
2. Set up a Railway account and obtain an authentication token.
3. Add the Railway token as a secret named `RAILWAY_TOKEN` in your repository settings.
4. Create Project name in `.github/workflows/main.yml` with your actual project name.
5. Commit and push the changes to your repository.

The CI/CD pipeline will automatically trigger on every push to the `main` branch, running tests and deploying the application to Railway if tests pass.
