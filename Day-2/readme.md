# Day-2
**September 10, 2024**
# Medusa Setup

## Prerequisites

Before you begin setting up Medusa, ensure you have the following:

### 1. Node.js and npm

- **Node.js**: Medusa requires Node.js. Download and install Node.js from [nodejs.org](https://nodejs.org/).
-  This will include npm (Node Package Manager).

  To verify installation, run:
  bash
  node -v
  npm -v
  

### 2. PostgreSQL

- Medusa uses PostgreSQL as its database. Install PostgreSQL from [postgresql.org](https://www.postgresql.org/download/)
  and ensure it is running.

  - **Database Creation**: Create a new database for Medusa.

### 3. Redis

- Redis is used by Medusa for caching and background job processing. Install Redis from [redis.io](https://redis.io/download/)
  and ensure it is running.

### 4. Git

- Git is needed for cloning the Medusa repository. Install Git from [git-scm.com](https://git-scm.com/downloads).

  To verify installation, run:
  bash
  git --version
  

### 5. Medusa CLI

- Install the Medusa CLI globally using npm:
  bash
  npm install -g @medusajs/medusa-cli
  

### 6. AWS Account (if deploying to AWS)

- If you plan to deploy Medusa on AWS, ensure you have an AWS account and the AWS CLI installed. Configure the AWS CLI with your
  credentials:
  bash
  aws configure
  

### 7. Terraform and AWS CLI (for Infrastructure as Code)

- If you're using Terraform for Infrastructure as Code (IaC), install Terraform from [terraform.io](https://www.terraform.io/downloads)
- and ensure the AWS CLI is installed as mentioned above.

### 8. Editor and IDE

- Have a text editor or IDE of your choice (e.g., VSCode, Sublime Text) for code editing.

## Next Steps

Once you have all the prerequisites installed, you can proceed with cloning the Medusa repository,
setting up the environment, and running Medusa.

### For efficient handling install Chocolatey to install other softwares and packages automatically with the command

bash
choco install <package-name>

# Today's Task

## Integrate and Run Medusa locally

### Make sure all the prerequisites are set

- node.js
- npm (node package manager)
- postgresql
- git

### Steps to follow

**Install the Medusa CLI**: Install the Medusa CLI globally using NPM
  
  bash
  npm install @medusajs/medusa-cli --global

**Setup postgresql database with default credentials or skip the process and setup your database details later on** 

**Create a Medusa Server Project**

  bash
  medusa new my-medusa-store

**Start the Medusa Server**

- Navigate to our medusa server project directory and start the server

  bash
  cd watch-store-medusa-server
  medusa develop

  *Test It Out*
  
  - Send a get request to the API’s products endpoint using curl in a different terminal window to confirm the server is running properly.

    bash
    curl localhost:9000/store/products

  

  
