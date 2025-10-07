## Azure SQL services and capabilities
Azure SQL is a collective term for SQL Server based databases in Azure
### Specific Azure SQL services include:
- **SQL Server on Azure Virtual Machines**
    - Runs full SQL Server in the cloud (no on-prem hardware needed).
    - It’s an IaaS (Infrastructure as a Service) solution.
    - Works like on-prem SQL Server — easy lift and shift migration.
    - Best for apps needing OS-level access or features not supported in PaaS.
    - Supports hybrid deployments (part on-prem, part in cloud).
    - Full admin control over SQL Server and OS.
    - Ideal for development/testing and fast migration.
    - Can scale up easily (add CPU, memory, disk) without reinstalling software.
      
      Business Benefits:
      - Use same tools and skills across on-prem and cloud.
      - Suitable when full managed service isn’t possible.
      - Still requires regular DB administration like on-prem systems.

- **Azure SQL Managed Instance**

    - Fully managed SQL Server instance in the cloud.
    - Supports multiple databases on one instance.
    - Automates backups, patching, monitoring, etc.
    - You control security, logins, and resource allocation.
    - Uses other Azure services (Storage, Event Hubs, Entra ID, Key Vault).
    - Encrypted communications for data protection.

  Use Cases:
    - Lift-and-shift on-prem SQL Server with less admin work.
    - Needed if your app uses linked servers, Service Broker, or Database Mail.
    - Use Data Migration Assistant (DMA) to check compatibility.
 
  Business Benefits:
    - Reduces admin workload (auto patching, backups, scaling).
    - High SQL Server compatibility (~100%).
    - Supports SQL logins and Microsoft Entra ID (Azure AD) authentication.
 
  - **Azure SQL Database – Simple Notes**

    - PaaS (Platform as a Service) – Microsoft manages everything (patching, updates, backups).
    - You create a logical server in the cloud to host single or pooled databases.
 
   Options

   1. Single Database

   - One independent database in the cloud.
   - Microsoft manages the server.
   - You can scale up/down as needed.
   - Serverless option auto-scales and charges only for use.

    2. Elastic Pool
 
   - Multiple databases share the same pool of resources.
   - Saves cost when workloads vary at different times.

    Use Cases

    - Best for low-cost, low-maintenance cloud databases.
    - Ideal for new cloud applications.
    - Suitable for systems with variable workloads and high availability needs.

    Business Benefits

    - Automatic updates, patching, backups.
    - Scalable and highly available (99.995%).
    - Point-in-time restore and geo-replication for disaster recovery.
    - Advanced threat protection and auditing for security.
    - Encryption for data at rest and in transit.
