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

To configure an SFTP server, you will need to set up the following parameters:

* **Port Number**: Determine the port number on which the SFTP server will listen for incoming connections. define the port number above 1024.

* **Number of Parallel Clients Supported**: Define the maximum number of simultaneous client connections that the SFTP service will allow. This value depends on the server's hardware capabilities and expected workload. It's important to ensure that the server can handle the specified number of concurrent clients efficiently.

* **Base Folder**: Set the base folder on the server where clients will have access and perform file operations. This folder acts as the root directory for the SFTP server and determines the starting point for file transfers. Configure the appropriate permissions for this folder, allowing clients to access and manage files within the defined scope.

* **User Credentials**:
    * **Keyboard Interactive Authentication (Username/Password)**: Determine the authentication method for users accessing the SFTP server. Keyboard interactive authentication prompts clients for a username and password during the connection process. You will need to configure user accounts with corresponding usernames and passwords for clients to authenticate successfully.
    
    * **Public Key Authentication**: Public key authentication is an alternative method that provides enhanced security. It involves generating public-private key pairs for clients and configuring the server to accept public keys for authentication. Clients will need to generate their key pairs and provide their public keys to the server administrator for configuration.

After the configuration, verify the connectivity by using the SFTP client software - WinSCP or Filezilla