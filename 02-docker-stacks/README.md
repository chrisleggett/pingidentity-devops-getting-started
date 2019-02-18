# Docker Stacks
This directory contains some examples that automate the manual steps taken in the Docker standalone directories

## How to
Note: ensure you have started docker swarm before deploying the stack by running `docker swarm init`

Run the `stack-start.sh` script and pass a stack yaml file

For example, `./stack-start.sh fullstack.yaml`

When finished with the stack, run `./stack-cleanup.sh` script and pass a stack yaml file to clean up your environment.

For example, `./stack-cleanup.sh fullstack.yaml`

## Yaml Files
* `basic1.yaml` - Deploy PingDirectory in a stack with mounted out volume
* `basic2.yaml` - Deploy PingDirectory in a stack with mounted in/out volumes
* `basic3.yaml` - Deploy PingDirectory in a stack with extenally mounted volumes
* `fullstack.yaml` - Deploy PingFederate, PingDirectory, PingDataConsole and PingAccess in a networked stack
* `simplest-sync.yaml` - Deploy PingDirectory, PingDataSync and PingDataConsole in a networked stack
