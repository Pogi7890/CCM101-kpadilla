# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture splits an application into two separate layers that communicate over a network. In this lab, one tier is the Nextcloud web application and the other is the MariaDB database.

## The Web/Application Tier

The web/application tier is what users interact with. It serves the user interface, handles HTTP requests from the browser, runs the application logic (such as logging in and uploading files), and asks the database tier for the data it needs. In this lab, the Nextcloud container fills this role.

## The Database Tier

The database tier stores persistent data such as user accounts, credentials, and file metadata. It receives queries from the application tier and returns results. In this lab, the MariaDB container fills this role.

## Why Separate Them?

Separating the web server and the database into two containers lets each be updated, scaled, restarted, and secured independently, so a problem in one does not necessarily bring down the other. It also follows the single-responsibility principle, which makes each container simpler to troubleshoot and lets the database be protected without being exposed to users.
