# Navjot Kaur Portfolio Website

This repository contains the source code for Na Feng's portfolio website, showcasing course work and projects. The website is built using React and packaged with Docker for easy deployment and execution.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Docker

## Getting Started

To get the web application running locally on your machine, follow these steps.

### Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/brainers12/react-portfolio.git
cd react-portfolio
```


### Build the Docker Image

From within the project directory, build the Docker image using the following command:

```bash
docker build -t navjot_kaur_coding_assignment14 .
```

This command builds a Docker image named `navjot_kaur_coding_assignment14` based on the instructions in the `Dockerfile`.

### Run the Container

Once the image is built, you can run the container using:

```bash
docker run -d -p 5575:5575 --name navjot_kaur_coding_assignment14_container navjot_kaur_coding_assignment14
```

This command starts a container named `navjot_kaur_coding_assignment14_container`, maps port 5575 on your host to port 5575 on the container, and runs in detached mode.

### Access the Application

The portfolio website should now be accessible at `http://localhost:5575`.

## Stopping the Container

To stop and remove the container when you're done, use:

```bash
docker stop navjot_kaur_coding_assignment14_container && docker rm navjot_kaur_coding_assignment14_container
```
