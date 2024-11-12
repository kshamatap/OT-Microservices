# Frontend POC
### This document provides Proof-of-Concept (POC) of frontend in detail.


| **Author** | **Created on** | **Last updated by** | **Last edited on** |
|------------|----------------|----------------------|---------------------|
| Kshamata      | 11-11-24      | Kshamata             | 12-11-24           |


## Purpose
The frontend web is a REACTJS based application which is user interface of [OT-Microservices](https://github.com/OT-MICROSERVICES) stack. This application supports cross-platform and can be executed on multiple OS as long as a JavaScript runtime environment is available. 
A ReactJS based web framework for the complete web page based operations
Test case integration for application functionality verification

## System Requirements
| System requirement | Minimum Requirement  |
|:-----------------------:|:--------------------:|
|  **OS**                 | Ubuntu or other Linux-based OS | 
| **Disk space**            | 20 GB    |
| **RAM**                 | 4 GB|
| **Processor**          | Dual-core recommended        |
| **Instance Type**        | t2.medium|

## Pre-requisites
- The frontend application have dependencies on other REST API of OT-Microservices like Employee, Attendance and Salary APIs which need to be configured.
- **Node.js**: Provides the runtime environment for executing JavaScript on the server-side and building and packaging React code.
- **NPM (Node Package Manager)**: Used to install, manage and run dependencies(java script libraries and tools) that the application depends upon.
NPM helps you manage these dependencies by adding them to a package.json file, which lists all the libraries our application depends on.

## Architecture

## Installation Steps
For the Frontend PoC, follow the steps mentioned below:

1. **Instance Creatiion**
After instance creation, first step is to update the packages (instance type t2.medium, volume 20GB)
```sh 
    sudo apt update
```

2. **Clone the Repository:**
    ```sh
    git clone https://github.com/OT-MICROSERVICES/frontend.git
    cd frontend
    ```
 ![Screenshot from 2024-11-11 14-06-33](https://github.com/user-attachments/assets/46374ed6-19ec-4466-adfa-ac21497c15e7)
 
3. **Create directory name `Public`** into frontend directory and create `index.html` file Where we have add following content.

```
html<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>React Frontend App</title>
</head>

<body>
  <div id="root"></div>
  <h1>Welcome to Frontend Web Page</h1>
</body>
</html>
```

4. **Edit the package.json file:**
In the `package.json` change the ip address with the public ip address in the proxy with specified port.

![Screenshot from 2024-11-11 14-11-07](https://github.com/user-attachments/assets/405c93ce-70e9-408c-be37-02762b769db9)

5. **Install nodejs:**

```sh 
    sudo apt update
    sudo apt install nodejs -y
```
![Screenshot from 2024-11-11 14-24-57](https://github.com/user-attachments/assets/d434936a-9f83-47b7-b8d1-fdc99e71012b)

6. **Build the application:**
For building the application. we can use make command from the Makefile.

```sh
    make build
```
![Screenshot from 2024-11-11 14-43-29](https://github.com/user-attachments/assets/90637463-04b1-46fb-b0a3-048b675ccfb7)

7. **Run the application:**
The command to run the application is as follows

```sh
    npm start
```
![Screenshot from 2024-11-11 15-45-38](https://github.com/user-attachments/assets/7231bd8b-0b8b-431a-b9bc-69843879deb9)

8. **Output:**
Finally we get the output by hitting the public ip of the VM:

![Screenshot from 2024-11-11 15-40-20](https://github.com/user-attachments/assets/a4e6d3af-73e9-4867-a3fb-5f04ceb47737)

##  Reference Links
| Links | Description      |
|-----  |--------------------------|
| https://nodejs.org/en/download/package-manager/all | For nodejs Installation | 
https://www.geeksforgeeks.org/how-to-install-node-js-and-npm-on-ubuntu/  | For NPM Installation
## Contact
| Name          | Email Address       |
|---------------|---------------------|
| Kshamata |  kshamata.prasad.snaatak@mygurukulam.co|
Collapse





















