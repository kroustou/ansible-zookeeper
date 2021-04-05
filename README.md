# Deploy zookeeper on Ubuntu

This playbook deploys zookeeper on X number of servers. The servers should be defined under the zookeeper group in the `hosts` file.

## Installation
To make sure your environment is functional please make sure to run `pip install -r requirements.txt`.

Next, update `hosts` to make sure all the servers are there. Note that zookeeper suggests that *a cluster should consist of 2n+1 number of servers*, so make sure to create at least 3 servers.

## Running the playbook
`ansible-playbook deploy.yml` should set up a cluster with the http server deactivated.
