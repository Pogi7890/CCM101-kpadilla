# Mission Reflection: Learning Cloud Security

Completing this laboratory showed me how quickly an unsecured cloud server can become vulnerable. A server may run its application correctly, but that does not mean it is safe. Administrators must identify exposed services, restrict unnecessary connections, and configure access rules before allowing users to connect.

A host-based firewall provides protection by checking network traffic on the server itself. It can reject unauthorized incoming connections even when another security layer has failed. This defense-in-depth approach is important because no single security measure can protect a system from every threat. A firewall works best alongside system updates, secure passwords, access controls, and monitoring.

Open network ports can increase a server's attack surface. Each accessible port may expose a service that contains weaknesses or has been configured incorrectly. Reducing the number of open ports makes it harder for attackers to find a useful entry point. During this mission, the goal was to permit only the connections required for administration and web access.

A publicly exposed database port, such as port 3306 for MySQL, creates additional risks. Unauthorized users could repeatedly attempt to log in, exploit outdated database software, or access private records if other protections fail. Databases should be isolated from direct public access whenever possible. Application servers should connect to them through restricted networks and approved firewall rules.

I also learned why firewall rules must be applied in the correct order. Allowing SSH before enabling UFW helps maintain remote access. A mistake in this step can interrupt administration and make recovery more difficult. Checking the firewall status and testing the web application are important ways to confirm that the configuration behaves as expected.

My GitHub portfolio demonstrates my progress through different cloud computing tasks, including deployment, operations, and security. This mission changed my perspective because I realized that security is not a one-time activity. It requires regular reviews, careful decisions, and continuous improvements to keep systems reliable and protected.
