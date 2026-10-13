

\# Docker Web Application Architecture



This diagram illustrates the local Docker environment used to deploy a custom Nginx web application.



```mermaid

flowchart TD

&#x20;   A\["Windows PC / Web Browser"]

&#x20;   B\["localhost:8081"]

&#x20;   C\["Docker Desktop / WSL 2"]

&#x20;   D\["Docker Container"]

&#x20;   E\["Nginx Web Server - Port 80"]

&#x20;   F\["Custom HTML/CSS Website"]



&#x20;   A --> B

&#x20;   B -->|"Port Mapping 8081:80"| C

&#x20;   C --> D

&#x20;   D --> E

&#x20;   E --> F

```



\## Architecture Overview



\- \*\*Windows:\*\* Hosts the Docker Desktop environment.

\- \*\*WSL 2:\*\* Provides the Linux environment for Docker.

\- \*\*Docker:\*\* Runs the containerized application.

\- \*\*Nginx:\*\* Serves the custom website.

\- \*\*Port Mapping:\*\* Connects localhost:8081 to container port 80.

\- \*\*HTML/CSS:\*\* Provides the website content.



