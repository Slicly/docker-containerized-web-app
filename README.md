

\# Docker Containerized Web Application



\## Project Overview

This project demonstrates how to containerize and deploy a custom web application using Docker and Nginx.



The application runs inside a lightweight Linux-based Docker container and is accessible through a local web browser.



\## Technologies Used

\- Docker Desktop

\- Docker Engine

\- Nginx

\- Alpine Linux

\- HTML/CSS

\- Windows PowerShell

\- Git and GitHub



\## Architecture



Windows Host

&#x20;   |

&#x20;   v

Docker Desktop (WSL 2 Backend)

&#x20;   |

&#x20;   v

Docker Container

&#x20;   |

&#x20;   v

Nginx Web Server (Port 80)

&#x20;   |

&#x20;   v

Custom HTML Website



Host Port: 8081

Container Port: 80



\## Implementation

1\. Installed and configured WSL 2 and Docker Desktop.

2\. Created a custom HTML/CSS website.

3\. Created a Dockerfile using Nginx Alpine.

4\. Built a custom Docker image.

5\. Deployed the application inside a Docker container.

6\. Configured port mapping to access the website locally.

7\. Used Git for version control and GitHub for source code hosting.



\## Docker Commands



Build the Docker image:



```bash

docker build -t my-cloud-website .

```



Run the container:



```bash

docker run -d -p 8081:80 --name cloud-website my-cloud-website

```



View running containers:



```bash

docker ps

```



Stop the container:



```bash

docker stop cloud-website

```



\## Accessing the Application



Open a browser and navigate to:



http://localhost:8081



The application runs locally and does not require AWS infrastructure.



\## Skills Demonstrated

\- Containerization

\- Docker image creation

\- Linux-based container environments

\- Web server deployment

\- Port mapping and networking

\- Infrastructure troubleshooting

\- Git version control



\## Application Screenshot



!\[Docker Website](docker-website.png)



\## Architecture Diagram



See the \[Docker Architecture Diagram](architecture.md) for a visual overview of the containerized application.



