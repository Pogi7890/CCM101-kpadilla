# Mission 6 Reflection

**1. Compose vs. manual commands**
Writing a docker-compose.yml file makes a cloud engineer's job easier because the whole setup lives in one file instead of many commands that I must remember and retype. With manual commands, one typo could break the deployment. With Compose, I run one command and get the same result every time. The file can also be saved on GitHub, shared, and reused, which is the core idea of Infrastructure as Code.

**2. Indentation errors in YAML**
YAML uses spaces to show which settings belong under which service. If I use a Tab instead of spaces, Docker Compose cannot read the structure and stops with a parsing error, so nothing is deployed until I fix it. This showed me that small formatting details matter a lot in configuration files.

**3. Why environment variables?**
Environment variables let us configure the containers without changing the images themselves. The database and Nextcloud must use the same credentials, so defining them in the Compose file keeps both services consistent. In a real production system, I would store secrets more safely, such as in a separate .env file that is not uploaded to GitHub.

**4. Deploying Nextcloud in minutes**
It felt impressive. Seeing the Nextcloud setup page appear after typing just one command made me realize how powerful containers and automation are, since installing this manually on a server would normally take much longer.

**5. Growth since Mission 1**
Since Mission 1, my understanding has grown from knowing what the cloud is to actually building and deploying services. I moved from basic concepts to containers, storage, and now multi-container applications. I now see the cloud as something engineers design, automate, and manage with code, not just a place to store files.
