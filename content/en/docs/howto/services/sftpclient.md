---
title: "SFTP Client"
lead: "Standalone Agents"
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "services"
weight: 101
toc: true
---

To configure file transfers based on SFTP client services, the below parameters should be configured:

* **IP Address and Port Number**: Provide the IP address and port number of the SFTP server. This information is necessary for the SFTP client to establish a secure connection with the server.

* **Specify Source and Target**: Specify the source folder (local directory) from where the files will be transferred, and the target folder (remote directory) on the SFTP server where the files should be uploaded or accessed.

* **Username and Password**: Enter the username and password credentials associated with the SFTP server. This is required for the client to authenticate and gain access to the server for file transfers. Alternatively public key based authentication information shall be configured

* **Scan Interval**: Determine the desired time interval for the client to perform scheduled transfers. The scan interval specifies how frequently the client will check for new or modified files to transfer. scan interval shall be minimum of 1 minute to maximum of 60 minutes.

* **Scheduled Transfer**: Set up the scheduled transfer feature in your SFTP client. The scheduling shall be provided based on crontab syntax

By configuring these parameters, you can set up file transfers using SFTP client to automate file transfers at specified intervals. The client will connect to the SFTP server using the provided IP address, port number, username, and password, and perform file uploads from the local source folder to sftp server target folder.