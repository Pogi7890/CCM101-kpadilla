# Mission Reflection

This laboratory activity helped me understand the difference between using a traditional Virtual Machine and using Docker containers. When using a Virtual Machine, an entire operating system must be installed and started before an application can run. This process can take more time and requires more system resources. In comparison, Docker containers share the host operating system kernel, so they can start much faster and use fewer resources. The Nginx container demonstrated how a web server can be deployed in only a few Docker commands.

Port mapping is necessary because the web server inside the container is listening on port 80, while the host needs a way to access that service. The command `-p 8080:80` connects port 8080 on the host to port 80 inside the container. This allowed me to access the Nginx web server by using `curl http://localhost:8080`. Without the port mapping, the Nginx service would not be directly accessible through port 8080 on the host.

When the `docker rm` command is used, the specified stopped container is removed from the Docker environment. Any data stored only inside the container can be lost when the container is removed. This shows why persistent application data should normally be stored using appropriate storage mechanisms such as Docker volumes rather than relying only on the container itself.

Containerization can also improve collaboration between software developers and IT operations teams. Developers can package applications and their dependencies into containers, while operations teams can run the same containerized application in different environments. This supports a more consistent deployment process and is an important part of DevOps practices.

My GitHub portfolio is evolving as I add more cloud computing activities and technical documentation. Laboratory 4 adds practical Docker and containerization experience to my previous cloud activities. Organizing the Markdown files and screenshots also helps make my portfolio easier to understand and demonstrates the skills I learned during the laboratory activity.
