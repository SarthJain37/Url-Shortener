
# URL Shortener

![License](https://img.shields.io/github/license/SarthJain37/Url-Shortener)
![Issues](https://img.shields.io/github/issues/SarthJain37/Url-Shortener)
![Forks](https://img.shields.io/github/forks/SarthJain37/Url-Shortener)
![Stars](https://img.shields.io/github/stars/SarthJain37/Url-Shortener)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction

Welcome to the URL Shortener project! This application allows you to shorten long URLs into concise, easy-to-share links. It's perfect for reducing the length of URLs for social media posts, emails, and other communications.

## Features

- **URL Shortening**: Convert long URLs into short, easy-to-share links.
- **Custom Aliases**: Create custom short links for easy recall.
- **Analytics**: Track the number of clicks on your shortened URLs.
- **RESTful API**: Use the API to integrate URL shortening into your own applications.

## Installation

### Prerequisites

- Python 3.1+
- pip (Python package installer)

### Steps

1. Clone the repository:
    ```bash
    git clone https://github.com/SarthJain37/Url-Shortener.git
    cd Url-Shortener
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up the database:
    ```bash
    python manage.py migrate
    ```

5. Run the application:
    ```bash
    python manage.py runserver
    ```

## Usage

After starting the server, navigate to `http://localhost:8000` in your web browser to access the URL Shortener interface. Here you can enter long URLs and receive shortened versions.

### API Usage

To use the REST API, you can send a POST request to the \`/api/shorten\` endpoint with the URL you wish to shorten. Example:

```bash
curl -X POST http://localhost:8000/api/shorten -d "url=http://example.com"
```

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (\`git checkout -b feature-branch\`).
3. Commit your changes (\`git commit -am 'Add new feature'\`).
4. Push to the branch (\`git push origin feature-branch\`).
5. Create a new Pull Request.

Please ensure your code follows the project's coding standards and includes relevant tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- [Django](https://www.djangoproject.com/) - The web framework used.
- [Bootstrap](https://getbootstrap.com/) - For responsive UI design.
- [Font Awesome](https://fontawesome.com/) - For icons.
