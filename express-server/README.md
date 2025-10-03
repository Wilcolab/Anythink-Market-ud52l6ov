# Express Server Project

This project is a simple Express server that listens on port 8001. It is set up to use `nodemon` for automatic code updates during development.

## Project Structure

```
express-server
├── src
│   └── index.js          # Entry point of the application
├── package.json          # Configuration file for npm
├── yarn.lock             # Dependency lock file
├── Dockerfile            # Dockerfile for containerization
└── README.md             # Project documentation
```

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository**:
   ```
   git clone <repository-url>
   cd express-server
   ```

2. **Install dependencies**:
   ```
   yarn install
   ```

3. **Run the server**:
   ```
   yarn start
   ```

The server will start and listen on `http://localhost:8001`.

## Docker

To run the server in a Docker container, build the Docker image using the following command:

```
docker build -t express-server .
```

Then, run the container:

```
docker run -p 8001:8001 express-server
```

The server will be accessible at `http://localhost:8001` from your host machine.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.