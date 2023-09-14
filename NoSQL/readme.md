# NoSQL Course resources
This folder contains resources for the NoSQL course.

## Setup
### A) with Docker installed locally
If you have Docker installed on your machine, the only thing you need is to download the `docker-compose.yml` file and run `docker-compose up -d` in the same folder as the file. This will download and start all the necessary containers.

### B) with Docker installed in a prepared Debian VM
1) Download the VM image from the following link: https://downloads.jetbrainer.com/db4.ova
2) Import the VM image into VirtualBox
3) Adjust the VM resources to your liking. The minimum requirements are 512MB of RAM and one vCPU, but for optimal performance it is recommended to use 2 vCPUs and 2GB of RAM.
4) Start the VM, you should then be able to access the databases on their default ports on the VM IP address

**In case you need to access or modify the VM**
- Username: `user`
- Password: `kaktusdelta`

Internally the VirtualMachine uses docker to host the databases, so you can use the same commands inside as if you had docker installed locally.
You can find the docker-compose.yml for the databases in the `/db4` folder.


## Databases
Following databases are available:

### Redis
- Port: `6379`
- No login required by default

### Cassandra
- Port: `9042`
- No login required by default

### MongoDB
- Port: `27017`
- User: `user`
- Password: `kaktusdelta`

### Neo4j
- Port: `7474`
- Dashboard port: `7687`
- User: `neo4j`
- Password: `kaktusdelta`