# AWS Services, Service Models, and Shared Responsibility

---

## I. AWS Core Service Introduction

| Term              | Definition / Role                                                                 |
|-------------------|-----------------------------------------------------------------------------------|
| AWS               | A group of cloud-based services offered by Amazon.                               |
| Access            | AWS services are accessed via the **Amazon Management Console**.                 |
| VM's (Instances)  | Virtual Machines in AWS are referred to as **Instances**.                        |
| EC2               | **Elastic Compute Cloud**: A core AWS service to launch and manage instances.    |
| Applications      | Client applications can be built using technologies like `.zip`, Java, .NET, Python.|

---

## II. The 3 T's of Cloud Computing

Fundamental benefits offered by AWS and other cloud providers:

- **Elasticity**:  
  Automatically scales resources up or down based on demand.

- **Scalability**:  
  Ability to handle growth by adding more resources when needed.

- **High Availability**:  
  Ensures applications remain accessible by distributing workloads across multiple systems.

---

## III. Cloud Service Models & Responsibility Layers

Understanding who is responsible for managing each layer in different service models.

### 1. Infrastructure as a Service (IaaS)

| Component                          | Responsibility       | Details & Implications                                                                 |
|-----------------------------------|----------------------|-----------------------------------------------------------------------------------------|
| Application, Data, OS             | Customer             | The customer manages the application, operating system, and data.                      |
| Network, Virtualization, DC, HW   | Provider (AWS)       | AWS manages physical infrastructure and the virtualization layer (hypervisor).         |
| AWS Security                      | Note                 | AWS **cannot access inside your VMs**, ensuring privacy and security.                  |
| AWS Example                       |                      | **EC2** (Elastic Compute Cloud)                                                        |

---

### 2. Platform as a Service (PaaS)

| Component                          | Responsibility       | Details & Implications                                                                 |
|-----------------------------------|----------------------|-----------------------------------------------------------------------------------------|
| Application, Data                 | Customer             | The customer manages their application code and data only.                             |
| OS, Virtualization, Network, DC  | Provider             | AWS manages everything below the application layer.                                    |
| AWS Example                       |                      | **Elastic Beanstalk** – Simplified app deployment.                                     |
| Other Example                     |                      | Microsoft **Azure**                                                                    |

---

### 3. Software as a Service (SaaS)

| Component                          | Responsibility       | Details & Implications                                                                 |
|-----------------------------------|----------------------|-----------------------------------------------------------------------------------------|
| Entire Stack (App, OS, HW, etc.) | Provider             | The cloud provider manages everything.                                                 |
| Customer Role                     |                      | Customer uses the app through a browser or client with no server maintenance required. |
| Examples                          |                      | **Gmail, WebEx, Zoom, Salesforce**                                                     |

---

## IV. Shared Responsibility Model

Defines who is responsible for **what** in a cloud environment:

- **Customer Responsibility**:  
  "Security **in** the Cloud"  
  - Managing your **Operating Systems**
  - Patching
  - Security Groups
  - Data Encryption
  - Access Control

- **Provider Responsibility**:  
  "Security **of** the Cloud"  
  - Physical infrastructure
  - Global data centers
  - Network hardware and virtualization

---

