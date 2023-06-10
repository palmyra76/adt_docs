---
title: "SFTP Server"
lead: "Standalone Agents"
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "services"
weight: 100
toc: true
---


An SFTP server enables secure file transfer between authenticated users, allowing them to upload and download files securely. It supports multiple users, granting them access to the server, and provides the option to automate file uploads using an agent.


**IP Address:** It is used by the SFTP server to listen for incoming connections from SFTP clients.

**Port Number:** It specifies the endpoint on the SFTP server for client connections.

**Base Folder:** The base folder in an SFTP server acts as the main folder where clients can access and manage files, determining their permissions and serving as the starting point for all file operations.

**User Information:** 

- The **Username** unique identifiers assigned to individual clients, distinguishing them from other users accessing the server.
- The **Password** the secret codes associated with each username, serving as a means of verifying the user's identity and granting access to their designated file directories.