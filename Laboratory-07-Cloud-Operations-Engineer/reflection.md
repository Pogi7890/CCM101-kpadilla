# Mission 7 Reflection

This laboratory activity helped me understand why monitoring is an important part of cloud computing. I learned that deploying an application is not enough because the server and its containers must also be checked to make sure they are working properly.

Checking the host server's resources is important even when the containers are running because the host provides the CPU, memory, and storage needed by those containers. If the server runs out of memory or disk space, the application may become slow or stop working. Checking these resources helps identify possible problems before they affect users.

The `docker logs` command is useful when a user reports that they cannot log in to a web application. The logs can show errors and requests handled by the application, which can help an engineer investigate what happened. However, the logs must be reviewed carefully because not every login problem will appear in the container logs.

Logs and metrics provide different types of information. Logs show individual events, requests, and errors, while metrics show measurements such as CPU usage and memory consumption. Using both makes it easier to understand whether a problem comes from an application error or from high resource usage.

Large enterprise companies can monitor thousands of containers by using centralized monitoring tools. Prometheus can collect and store metrics, while Grafana can display them through dashboards. These tools help operations teams observe many services and identify unusual behavior without checking every container manually.

My troubleshooting skills improved through using Linux commands and Docker tools to examine the server and the web application. I learned how to check memory and disk capacity, deploy an Nginx container, send HTTP requests, generate a 404 error, and inspect logs and resource metrics. This activity also showed me the importance of collecting evidence and recording actual results. In future cloud projects, I will use these monitoring techniques to investigate problems more systematically instead of relying only on assumptions.
