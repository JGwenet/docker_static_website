# README.md

# Static Website with Docker

This project is a simple static website that can be deployed using Docker. It includes an HTML file as the main entry point and a Dockerfile to build the Docker image.

## Project Structure

```
static-website
├── src
│   └── index.html
├── Dockerfile
├── .dockerignore
└── README.md
```

## Files

- `src/index.html`: Contains the HTML markup for the static website.
- `Dockerfile`: Instructions to build the Docker image for the static website.
- `.dockerignore`: Specifies files and directories to ignore when building the Docker image.

## Getting Started

To build and run the Docker container for this static website, follow these steps:

1. **Build the Docker Image**

   Run the following command in the project root directory:

   ```
   docker build -t my-static-website .
   ```

2. **Run the Docker Container**

   After the image is built, run the container using:

   ```
   docker run -d -p 8080:80 my-static-website
   ```

3. **Access the Website**

   Open your web browser and go to `http://localhost:8080` to view the static website.
