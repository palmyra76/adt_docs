---
title: "Quick Start"
description: "Enroll, install and configure agents and start transfer files"
lead: "Enroll, install and configure agents and start transfer files"
date: 2020-11-16T13:59:39+01:00
lastmod: 2020-11-16T13:59:39+01:00
draft: false
images: []
menu:
  docs:
    parent: "overview"
weight: 110
toc: true
---

### Enroll in Transyra.com

### Install Agent
* **Create an Agent Configuration**: In the central console, create an agent configuration specifying the agent name and agent type and save the configuration.
* **Download the Agent**: Once the agent configuration is created, you will typically have an option to download the agent software. Click on the provided link to initiate the download. Save the downloaded file to a location on your system.
* **Register the Agent**: Open a terminal or command prompt and navigate to the directory where you downloaded the agent. Execute the registration command using the provided key. 
<br>
    ``` register_transyra.sh -key <generated_key> ```
<br> 
Replace <generated_key> with the actual key provided to you. This command registers the agent with the central console, establishing a connection between them.

* **Start the Agent**: After successful registration, start the agent by running the start command
<br>
    ``` start_transyra.sh ```
<br>
This command initiates the agent and connects it to the central console, allowing it to receive instructions and perform file transfer tasks.

### Configure Agent

To add commonly available services and configure additional agents for file transfers between them, follow these steps:

1. **SFTP Server/Client**: Configure an SFTP server on the agent. This server will allow secure file transfer using the SFTP protocol. Additionally, using SFTP clients like WinSCP or FileZilla on other machines to connect to the SFTP server and perform file transfers.

3. **TUS Server/Client**: TUS is a protocol for resumable file uploads over HTTP. using TUS Server and client configuration, Site2Site transfer files are configured with resumable capabilities.

4. **Configure Additional Agents**: Install and configure additional agents on different machines. Follow the steps mentioned earlier in the "Install Agent" section to set up these agents and register them with the central console. Ensure that the agents are connected to the central console and listed as registered entities.

5. **Test File Transfers**: With the agents and services set up, you can now initiate file transfers between them. Use tools like WinSCP or FileZilla to connect to the agents and perform transfers. Configure the client tools to connect to the appropriate server and transfer files between agents.

By following these steps, you can add commonly available services such as SFTP, HTTP, and TUS, and configure additional agents to facilitate file transfers between them. This allows you to explore different transfer protocols and test file transfer scenarios.