# Simple Express Server

This project is a simple Express server that listens on port 8001. It is designed to demonstrate the use of Docker and nodemon for automatic server restarts during development.

## Project Structure

```
simple-express-server
├── src
│   └── server.js        # Entry point of the application
├── package.json         # Configuration file for npm
├── yarn.lock            # Dependency version lock file
├── Dockerfile           # Instructions to build the Docker image
└── README.md            # Project documentation
```

## Getting Started

### Prerequisites

- Node.js and npm (or Yarn) installed on your machine.
- Docker installed on your machine.

### Installation

1. Clone the repository:

   ```
   git clone https://github.com/microsoft/vscode-remote-try-node.git
   cd simple-express-server
   ```

2. Install dependencies:

   Using npm:
   ```
   npm install
   ```

   Or using Yarn:
   ```
   yarn install
   ```

### Running the Server

To start the server with automatic restarts on code changes, use:

```
yarn start
```

The server will listen on port 8001.

### Building the Docker Image

To build the Docker image, run:

```
docker build -t simple-express-server .
```

### Running the Docker Container

To run the Docker container, use:

```
docker run -p 8001:8001 simple-express-server
```

The server will be accessible at `http://localhost:8001`.

## License

This project is licensed under the MIT License.