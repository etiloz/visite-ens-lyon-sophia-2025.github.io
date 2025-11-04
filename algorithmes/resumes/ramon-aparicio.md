---
layout: default
title: Exposés de R. Aparicio-Pardo
---


## Can flexible AI workloads to stabilise electrical grids ? 

Renewable microgrids can help data centers cope with the increasing demand for cloud-based services, but they pay the price of the double uncertainty of workload and renewable resource availability.  The mismatch between demand and renewable supply prevents microgrid-based data centers from achieving full autonomy, requiring connection to the main grid. However, while imports from the main grid could increase environmental impact, the massive export of excess renewables, when injected into the grid, can cause serious instability in the system. This presentation proposes to address both issues using AI compressible tasks, whose potentially concave utility functions allow for the adaptation to the available resources, reducing or increasing the task size with negligible impact on the quality provided to the user. By absorbing surplus renewable energy, they help maintain frequency stability in the main grid, thereby supporting grid-forming operations. 


## Quantum Network AI-based Control 
In the long term, Quantum Communications promise to connect Quantum Processors placed at remote locations, giving rise to Quantum Cloud able to perform very complicated computation tasks in very shorter processing times. In the short term, Quantum Communications are applied in tasks such as cryptography key distribution or clock synchronization. In both cases, the basic “operation” necessary to carry out is the quantum entanglement distribution between the source and the destination of the communication. That is equivalent to packet forwarding in classical packet switched networks, and renamed as quantum datagram forwarding.

In this project, we aim to study the optimization of quantum (q-)datagram forwarding in connectionless quantum networks, that necessitates dynamic, real-time control strategies capable of managing inherent probabilistic processes and decoherence effects. Within a connectionless quantum network, the forwarding of a quantum request is abstracted into a series of sequential decisions made by intermediate nodes (quantum repeaters). These decisions focus primarily on optimizing the management of quantum resources, including when to attempt probabilistic operations like entanglement generation, when to execute entanglement swapping to extend the path, and how to utilize constrained quantum memory. 

Then, we aim to find optimal control policies for q-datagram forwarding that maximizes an objective (e.g., fidelity or rate) under real-time constraints.  These management decisions (i.e., control policies) constitute stochastic control problems, that can be modelled as Markov Decision Processes (MDPs) and solved under the Reinforcement Learning (RL) framework.
