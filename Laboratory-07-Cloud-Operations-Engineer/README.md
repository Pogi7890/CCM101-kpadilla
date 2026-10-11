# Mission 7: The Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on monitoring a Linux host and a containerized web application. Using KillerCoda and Docker, the Nginx web server was deployed, test HTTP requests were generated, application logs were examined, and container resource usage was monitored.

## Objectives

* Check the host's memory and disk capacity.
* Observe running processes and CPU activity using Linux tools.
* Deploy an Nginx container named `client-website`.
* Generate successful HTTP requests and an intentional 404 error.
* Examine application logs using `docker logs`.
* Monitor CPU and memory consumption using `docker stats`.
* Document the results and evidence in a GitHub portfolio.

## Monitoring Commands Executed

| Command                                                | Purpose                                    |
| ------------------------------------------------------ | ------------------------------------------ |
| `free -h`                                              | Check RAM usage and availability           |
| `df -h /`                                              | Check root filesystem capacity             |
| `top`                                                  | Observe running processes and CPU activity |
| `docker ps`                                            | Check running containers                   |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx web server                |
| `curl`                                                 | Generate HTTP requests and test responses  |
| `docker logs client-website`                           | Inspect application logs                   |
| `docker stats`                                         | Monitor container resource usage           |

## Skills Learned

This activity provided practice in Linux system monitoring, Docker container deployment, HTTP testing, log analysis, and resource monitoring. It also demonstrated how screenshots and Markdown reports can document technical results in a GitHub portfolio.

## Evidence

The `screenshots/` folder contains the terminal evidence collected during the activity, including the host baseline, Nginx deployment, HTTP responses, application logs, and container metrics.

## Conclusion

Monitoring the host and its containers helps cloud operations engineers identify errors and observe resource consumption. Combining system information, application logs, and container metrics supports more informed troubleshooting and performance assessment.
