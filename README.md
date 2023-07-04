# 🌊 Raft

Raft is a simple implementation of the Raft distributed consensus algorithm in Go. It provides a reliable and fault-tolerant system for achieving consensus among a group of nodes in a distributed network. This project aims to implement the core functionalities of the Raft algorithm, allowing for leader elections, commands/log replication, persistence, membership changes, and log compaction.

The Raft algorithm, introduced in the paper [link](https://raft.github.io/raft.pdf), is designed to handle the challenges of maintaining consensus in a distributed system. It ensures that all participating nodes agree on the state of the system, even in the presence of failures or network partitions.

## Todo

The project's roadmap includes the following tasks:

- [ ] Leader elections: Implement the leader election mechanism, where nodes in the network elect a leader among themselves to coordinate the consensus process.

- [ ] Commands/Log replication: Develop the functionality to replicate commands and log entries across the nodes in the system. This ensures that all nodes have a consistent view of the system's state.

- [ ] Persistence: Implement persistence mechanisms to store the replicated logs and system state on disk. This allows the system to recover from failures and resume operations seamlessly.

- [ ] Membership Changes: Handle dynamic changes in the network membership, such as adding or removing nodes. Implement mechanisms to ensure a smooth transition without compromising the system's integrity.

- [ ] Log Compaction: Develop a log compaction mechanism to remove redundant or unnecessary log entries, improving system performance and reducing storage requirements over time.

## K-v Implementation

In addition to the core Raft algorithm, the project aims to build a distributed key-value (K-v) store using the Raft consensus algorithm. This K-v store will leverage the reliability and fault tolerance provided by Raft to ensure consistent and durable access to key-value pairs across the distributed network.

By implementing a K-v store on top of the Raft consensus algorithm, the project aims to provide a highly available, scalable, and fault-tolerant solution for distributed key-value storage.

Overall, the Raft project seeks to provide a robust distributed consensus algorithm and a practical application in the form of a distributed key-value store. It combines the theoretical foundations of the Raft algorithm with a concrete implementation, demonstrating the power and effectiveness of consensus algorithms in distributed systems.
