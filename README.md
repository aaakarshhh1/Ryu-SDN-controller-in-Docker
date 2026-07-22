# Ryu SDN Controller in Docker

This project demonstrates how to deploy and manage a Ryu Software Defined Networking (SDN) controller inside a Docker container. The setup provides a lightweight and isolated environment for developing, testing and experimenting with OpenFlow-based SDN applications without requiring a native Ryu installation.

The project was built as part of an SDN laboratory exercise to better understand controller deployment, Docker containerization and OpenFlow communication between switches and the controller.

---

## Features

- Deploys the Ryu SDN Controller inside a Docker container
- Isolated and portable environment using Docker
- Supports OpenFlow-based SDN applications
- Easy setup without installing Ryu directly on the host machine
- Suitable for Mininet integration and SDN experiments
- Simplifies controller testing and development

---

## Technologies Used

- Python
- Ryu SDN Framework
- Docker
- OpenFlow
- Linux

---

## Project Structure

```
.
├── Dockerfile
├── docker-compose.yml
├── ryu_controller.py
├── requirements.txt
└── README.md
```

---

## How it Works

The Docker container runs the Ryu SDN Controller, which acts as the centralized control plane in a Software Defined Network. OpenFlow switches establish a connection with the controller, allowing it to receive packet events, install forwarding rules and manage network behavior dynamically.

Running the controller inside Docker makes the environment portable, reproducible and easy to deploy across different systems.

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/aaakarshhh1/Ryu-SDN-controller-in-Docker.git
cd Ryu-SDN-controller-in-Docker
```

### Build the Docker image

```bash
docker build -t ryu-controller .
```

### Run the container

```bash
docker run -it --rm -p 6633:6633 -p 6653:6653 ryu-controller
```

---

## Learning Outcomes

Through this project I gained practical experience with:

- Docker containerization
- Software Defined Networking concepts
- Ryu SDN Controller
- OpenFlow protocol
- Controller deployment and testing
- Linux networking fundamentals

---

## Future Improvements

- Integrate Mininet topologies
- Implement custom Ryu applications
- Add network monitoring and traffic visualization
- Deploy multiple controllers for scalability testing
- Integrate REST APIs for controller management

---

Developed as part of an academic SDN networking project.
