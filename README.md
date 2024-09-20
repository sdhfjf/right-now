# right-now

This project is a decentralized peer-to-peer (P2P) static website that operates using a single HTML file. The website allows seamless communication and peer discovery by sharing just one initial peer ID. Once a peer ID is known, it is automatically propagated and shared among other peers, ensuring smooth and efficient connectivity across the network.

## Key Features

- **Single HTML File**: The entire site is contained in one HTML file, making it lightweight and easy to deploy.
- **Peer Discovery**: After connecting to the network with a known peer ID, the system automatically shares this ID with other peers, creating a distributed network without requiring manual sharing.
- **P2P Communication**: The website supports direct communication between peers, eliminating the need for a central server and promoting a decentralized architecture.
- **Automatic Propagation**: Once connected, the initial peer ID is continuously propagated between all participants, ensuring automatic peer discovery and connectivity without further user input.

## Problems

1. **Scalability**: As the number of peers grows, the system may struggle with scaling efficiently. Managing larger peer groups could introduce issues with synchronization, peer discovery delays, and network overhead.
   
2. **STUN Server Requirement**: The P2P network  relies on a STUN server for peer discovery. However, the STUN server might not always be available, and when it is, it is often used inefficiently, leading to unnecessary bottlenecks and overhead in peer communication.

3. **Poor Network Approach**: The current networking strategy may not be optimal for handling dynamic connections, NAT traversal, and peer management. This could result in suboptimal performance, especially in environments with variable network conditions, high latency, or restrictive firewalls.
