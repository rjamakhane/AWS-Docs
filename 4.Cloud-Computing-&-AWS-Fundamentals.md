# Cloud Computing & AWS Fundamentals

---

## I. Core Definition: Cloud Computing

**Concept:**  
Computing done in a remote location ("the Cloud") instead of on-premises (local machine/data center).

**Transformation Path:**  
`Physical DC → Virtualization → CLOUD → AWS [Remote Location (Data Centers)]`

---

## II. Amazon Web Services (AWS)

**Role:**  
AWS is a Cloud Provider that offers a wide range of services.

**Key Offering:**  
Infrastructure as a Service (IaaS)

**Infrastructure:**  
AWS operates in approximately **33 Regions** globally.

**Access:**  
Cloud resources are accessed via the **internet** using the **AWS Management Console**.

### Global Infrastructure Terms

| Term              | Definition                                                            |
|-------------------|----------------------------------------------------------------------|
| Remote Location   | A geographical area (e.g., Mumbai, Hyderabad) containing infrastructure |
| Data Centers      | Physical buildings within a Remote Location                           |
| Infrastructure    | Components within data centers: Storage, Databases, Servers, Networks, VMs, etc. |

---

## III. Key Words & Concepts

| Term           | Role / Description                                           |
|----------------|--------------------------------------------------------------|
| Virtualization | Technology to run multiple VMs on a single host machine      |
| Hypervisor     | Software that manages and runs virtual machines              |
| Load Balancer  | Distributes traffic across servers                           |
| Firewall       | Network security system controlling inbound/outbound traffic|
| DNS            | Translates domain names into IP addresses                    |
| Protocols      | Rules for communication (e.g., TCP/IP)                       |
| Webservers     | Software/hardware for serving web content                    |
| On-premises    | Resources hosted locally by the organization                 |

---

## IV. Cloud Service Models

These define **who manages what** between the provider and the user.

| Model                        | Abbreviation | Focus                                | User Manages...              |
|-----------------------------|--------------|--------------------------------------|------------------------------|
| Infrastructure as a Service | IaaS         | VMs, Storage, Networks (foundation)  | OS, Applications, Data       |
| Platform as a Service       | PaaS         | Dev & deployment environment         | Applications, Data           |
| Software as a Service       | SaaS         | Complete, ready-to-use application   | Usage, Data                  |

---

## V. Deployment Models (Types of Clouds)

These define **where** the cloud is hosted and **who** can access it.

| Model         | Access & Ownership                                                    | Examples                                  |
|---------------|------------------------------------------------------------------------|-------------------------------------------|
| Public Cloud  | Accessible by anyone via internet. Provider owns infrastructure.       | AWS, Azure, Google Cloud Platform (GCP)   |
| Private Cloud | Used only by a single organization. Infrastructure is private.         | Oracle, IBM (Organizational Instances)    |
| Hybrid Cloud  | Combination of Public & Private. Often used to scale or integrate.     | Internal apps + scalable public services  |

---
