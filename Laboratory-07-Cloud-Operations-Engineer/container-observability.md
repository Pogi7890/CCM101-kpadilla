# Container Observability Report

## 1. Overview

This report documents the monitoring of the Nginx web server container named `client-website`. The activity covers HTTP traffic, application logs, and real-time resource metrics.

## 2. Web Traffic Results

Three HTTP requests were sent to the Nginx server.

* **Request 1:** HTTP 200
* **Request 2:** HTTP 200
* **Request 3:** HTTP 200
* **Missing page request:** HTTP 404

The successful responses indicate that Nginx served the requested pages, while the 404 response indicates that the requested path was not found.

## 3. Application Log Analysis

**Log entry showing the 404 error:**

```text
<html>
<head><title>404 Not Found</title></head>
<body>
<center><h1>404 Not Found</h1></center>
<hr><center>nginx/1.31.6</center>
</body>
</html>
```

Application logs are important for troubleshooting because they show the requests received by the application and the responses returned to users. They help engineers identify errors, trace problems, and determine what needs further investigation.

## 4. Real-Time Container Metrics

The Docker statistics dashboard was used to monitor the `client-website` container.

* **Container Name:** `client-website`
* **Memory Usage:** 2.738MiB
* **CPU Percentage:** 0.00% 

These measurements describe the container's resource consumption at the time of observation.

## 5. Evidence

* `screenshots/install-nginx.png`
* `screenshots/simulation1.png`
* `screenshots/simulation2.png`
* `screenshots/docker-logs.png`
* `screenshots/container-metrics.png`

## 6. Conclusion

Application logs help explain individual requests and errors, while container metrics show resource consumption. Using both provides a clearer picture of the web server's behavior and health.
