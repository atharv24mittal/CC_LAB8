# Raft Consensus Algorithm using Docker

## Aim
To implement a distributed system using the Raft consensus algorithm and observe leader election, fault tolerance, and quorum behavior.

## Technologies Used
- Python
- Docker
- Raftos Library

## Setup Instructions

### Step 1: Clone Repository
git clone <your-repo-link>
cd raft_docker_lab


### Step 2: Build and Run

docker-compose up --build


### Step 3: Observe Logs

docker logs -f node1
docker logs -f node2
docker logs -f node3
docker logs -f node4
docker logs -f node5


## Observations
- One node becomes leader
- Others act as followers
- System continues working with majority nodes
- System fails when majority is lost

## Key Concept
Raft requires majority (quorum) to elect a leader.

For 5 nodes:
Majority = 3

## Conclusion
The experiment demonstrates leader election, fault tolerance, and quorum behavior in distributed systems using Raft.

HOW TO PUSH TO GITHUB
Step 1:
git init
git add .
git commit -m "Raft Docker Lab - 5 Node Cluster"
Step 2:
git branch -M main
git remote add origin <your-repo-link>
git push -u origin main
