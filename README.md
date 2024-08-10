# Segment3D Deploment Master

This project is a part of the Segment3D project that could help us deploying all service just with one script execution

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)
  - [Running with Docker Compose in Local Machine](#running-with-docker-compose-in-local-machine)
  - [Running with Docker Compose in Virtual Machine](#running-with-docker-compose-in-virtual-machine)
  - [Stop the application](#stop-the-application)
  - [API Documentation](#api-documentation)
- [License](#license)

## Getting Started

### Prerequisites

Ensure you have the following tools installed on your machine:
- **Docker**: You can download it from [docker.com](https://www.docker.com/).
- **Docker Compose**: Docker Compose is used for defining and running multi-container Docker applications. It typically comes bundled with Docker Desktop, but you can also install it separately. See [Docker Compose installation guide](https://docs.docker.com/compose/install/) for more details.


### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/segment3d-app/deployment-master.git
    cd deployment-master
    ```

### Configuration
All configuration could you find in `.env` file

## Usage

### Running with Docker Compose

You can run the entire application using Docker Compose. This will set up the necessary containers for the backend and any other services you may have.

1. **Build and start the application using Docker Compose in Local Machine:**

   ```bash
   ./script/local-setup.sh
   ```

2. **Build and start the application using Docker Compose in Virtual Machine:**

   ```bash
   ./script/setup.sh
   ```

3. **Stop the application:**

   ```bash
   docker-compose down
   ```

### API Documentation

To access the API documentation, visit the Swagger documentation at `http://<vm-ip-address>:8080/swagger/index.html` (backend) and `http://http://localhost:8080/swagger/index.html:8081/swagger/index.html` (storage) after running the above script.

## License

This project is licensed under the [MIT License](LICENSE).
