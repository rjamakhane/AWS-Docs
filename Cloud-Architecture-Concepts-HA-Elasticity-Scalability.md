# ☁️ Cloud Architecture Concepts: HA, Elasticity, & Scalability

---

## I. High Availability (HA)

**Definition:**  
High Availability (HA) refers to the **percentage of time** a service is accessible to customers.

- **Available Period:** When the service is accessible.
- **Unavailable Period (Downtime):** When the service is **not** accessible.

**Goal:**  
The ultimate goal is **zero downtime**, which is achieved using:

- **Auto-Scaling**
- **Fault Tolerance**

### HA Components and Implementation (via Load Balancer)

High Availability is achieved through the combination of:

1. **Redundancy:**  
   - Deploying **duplicate instances** of the application on different servers.

2. **Monitoring (Health Checks):**  
   - The **Load Balancer (LB)** checks the application's availability using health checks.  
   - Example: Verifying if `/index.html` returns a **200 OK** status code.  
   - Health checks are done **on the application**, not the server.

3. **Failover:**  
   - If one server fails the health check, the LB routes traffic to a healthy server.  
   - The **Load Balancer performs the failover** automatically.

### Load Balancer in High Availability

- The user (e.g., Aman) accesses the application via a **single DNS** (e.g., `http://aman.com`).
- The Load Balancer distributes traffic to healthy backend servers.
- It may use strategies like **Round Robin** to balance traffic.
- Health checks are performed on backend servers (e.g., IPs `192.168.10.20`, `192.168.10.21`).

---

## II. Elasticity

**Definition:**  
Elasticity is the ability to **automatically increase or decrease** the number of computing resources (servers/instances) based on demand.

- **Time Frame:** Elasticity is a **short-term** capability.
- **Implementation in AWS:** Achieved using **Auto-Scaling Groups**.

### Auto-Scaling Actions

- **Scale Out:**  
  Increase the number of instances during high load.

- **Scale In:**  
  Decrease the number of instances during low load.

### Scaling Type

- **Horizontal Scaling:**  
  Elasticity is a form of **horizontal scaling**, meaning you add or remove entire servers.
  - Example: Adding multiple 4GB RAM servers to handle additional load.

---

## III. Scalability

**Definition:**  
Scalability is the ability to **increase the capacity** (CPU, RAM, Storage) of a **single server** or instance.

- **Time Frame:** Scalability is a **long-term** planning strategy.
- **Implementation in AWS:** Achieved by **changing the instance type**.

### Scaling Actions

- **Scale Up:**  
  Increase the capacity (e.g., upgrade from 8GB to 32GB RAM).

- **Scale Down:**  
  Decrease the capacity (e.g., downgrade from 32GB back to 8GB RAM).

### Scaling Type

- **Vertical Scaling:**  
  This is also called **vertical scaling**, where one server grows in power.

### Application Example

- Common for use cases like **Databases**, which are often not easily distributed:
  - E.g., A **single DB server** with 100 databases and 10TB of data is more suitable for vertical scaling.

---
