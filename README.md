# Skynet Scheduling Strategy in Cloud Platform
Skynet Scheduling and Monitoring System Overview
Skynet Scheduling and Monitoring System is a three-dimensional monitoring platform provided by Huawei Cloud Cloud Monitoring for elastic cloud servers, bandwidth, and other resources. Through this system, users can achieve real-time job monitoring and management, including job status monitoring, configuring event scheduling, setting variables, and displaying execution plans.

Real-time Job Monitoring
In the left navigation bar of the main interface for data development, select "Operations and Scheduling Job Monitoring", then click on the "Real-time Job Monitoring" tab to view detailed information about the job and monitoring data.

Event Scheduling and Configuration
On the "Child Job Monitoring" page, various operation options are provided in the "Actions" column, including stopping running child job instances, setting parameters needed for sessions or transactions, displaying execution plans, etc.

Applications in the Skynet framework
The Skynet framework ensures efficient operation of services through its unique service scheduling mechanism. In Skynet services, a new thread can be opened to handle business, and these threads are actually simulated by coroutines, avoiding the overhead of traditional threads.

Service Scheduling Mechanism
The Skynet service scheduling involves service sleeping, thread usage, execution authority management, execution authority concession, and timer management. Timers are used very frequently in Skynet, allowing services to execute tasks after a specific time or periodically.

Message Scheduling Model
The core part of Skynet is a message scheduling mechanism, in which several Worker threads are running. These threads take messages from the message queue and find the corresponding processing functions to distribute. In addition, Skynet also includes a Timer thread for implementing timing mechanisms, as well as a Socket thread for listening to epoll events and managing network operations.

Affinity and Anti-Affinity Scheduling Strategies
When creating container applications, Skynet supports setting affinity/anti-affinity scheduling strategies, such as deploying a certain type of application to specific nodes or deploying different applications to different nodes to achieve effective resource utilization and management.

Application scenarios of scheduling strategies
The affinity scheduling strategy allows container applications to be scheduled only on nodes that are affinitive with them, while the anti-affinity scheduling strategy is used to avoid scheduling container applications on specific nodes, thereby enhancing the flexibility and reliability of the system.

DDoS Ladder Scheduling Strategy
When you purchase DDoS native protection and enable joint protection, you can configure the DDoS step-up scheduling strategy to automatically trigger DDoS high defense to protect the protected resources, defending against massive attacks.

Advantages of the strategy
The DDoS ladder scheduling strategy can automatically link and schedule DDoS high defense resources when massive attacks occur, effectively protecting cloud resources from being affected by attacks, and ensuring the stability and availability of services.

Summary
The Skynet framework provides users with powerful resource management and job monitoring capabilities through its efficient scheduling strategies and mechanisms. Whether it's monitoring and managing real-time jobs or applying affinity and anti-affinity scheduling strategies, Skynet can help users achieve optimized resource allocation and efficient operation in cloud platforms.
