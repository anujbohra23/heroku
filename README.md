# Heroku Deployment Project

This repository contains a sample project to demonstrate how to deploy an application to Heroku. The project showcases the deployment of a Python web application using the Flask framework.

## Specifications and Tech Stack

- **Programming Language**: Python
- **Web Framework**: Flask
- **Deployment Platform**: Heroku
- **Dependencies**: Flask, Gunicorn, and other Python libraries as listed in `requirements.txt`
- **Procfile**: Defines the commands to run the application on Heroku

## Features

- Simple web application demonstrating basic routing with Flask
- Configured to run on Heroku with a `Procfile` and `requirements.txt`
- Instructions for local setup and deployment to Heroku

## Prerequisites

- Python 3.6 or higher
- pip (Python package installer)
- Heroku CLI

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/anujbohra23/heroku.git
    cd heroku
    ```

2. Create and activate a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Running the Application Locally

1. Set the `FLASK_APP` environment variable:
    ```bash
    export FLASK_APP=app.py  # On Windows use `set FLASK_APP=app.py`
    ```

2. Run the Flask application:
    ```bash
    flask run
    ```

3. Open your web browser and navigate to `http://127.0.0.1:5000/` to see the application in action.

## Deploying to Heroku

1. Login to Heroku:
    ```bash
    heroku login
    ```

2. Create a new Heroku app:
    ```bash
    heroku create your-app-name
    ```

3. Push the code to Heroku:
    ```bash
    git push heroku main
    ```

4. Open your application in the browser:
    ```bash
    heroku open
    ```

## Repository Structure

- `app.py`: The main application file containing the Flask routes
- `requirements.txt`: Lists the dependencies required to run the application
- `Procfile`: Specifies the commands to run the application on Heroku
- `runtime.txt`: Specifies the Python version to be used on Heroku

## Contributing

Feel free to fork this repository and make your own changes. Pull requests are welcome.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Flask Documentation](https://flask.palletsprojects.com/)
- [Heroku Documentation](https://devcenter.heroku.com/)
