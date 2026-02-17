# Region vs Availability Zone (AZ)

AWS resources are deployed in **Regions** and **Availability Zones (AZs)** to ensure high availability, fault tolerance, and low latency.

## 🌍 Region
- A **geographical location**, such as:
  - US East (N. Virginia)
  - Asia Pacific (Mumbai)
- Each Region is **independent** and contains multiple Availability Zones.
- Choose a Region based on:
  - Proximity to your users (low latency)
  - Compliance requirements
  - Cost considerations

## 🏢 Availability Zone (AZ)
- A **physically separate data center** within a Region.
- Each AZ is isolated but connected to other AZs in the same Region via **low-latency links**.
- Example:
  - Asia Pacific (Mumbai) Region:
    - ap-south-1a
    - ap-south-1b
    - ap-south-1c

---

## 🚀 Why Regions and AZs Matter

- **High Availability:**  
  Deploy resources across multiple AZs to maintain uptime during failures.

- **Low Latency:**  
  Select Regions closer to your users to reduce network delay.

- **Cost Optimization:**  
  Some Regions offer lower pricing for the same services.

---

# Introduction to EC2 Service

**Amazon Elastic Compute Cloud (EC2)** is a core AWS service used to deploy scalable virtual servers in the cloud.

## 🔹 Key Features

- **Scalability:**  
  Easily scale instances up or down based on demand.

- **Customizable Instances:**  
  Choose instance types based on CPU, memory, and storage requirements.

- **Secure Access:**  
  Use SSH key pairs and Security Groups to control access securely.

---

# EC2 Purchasing Options

AWS provides multiple pricing models to meet different workload needs:

## 1️⃣ On-Demand Instances
- No upfront payment or long-term commitment.
- Pay per second or per hour.
- Ideal for short-term, irregular, or unpredictable workloads.

## 2️⃣ Savings Plans
- Offers up to **72% savings** compared to On-Demand.
- Requires commitment to a consistent usage amount ($/hour) for 1 or 3 years.
- Most flexible discount option.

## 3️⃣ Reserved Instances (RI)
- Provides up to **72% discount** compared to On-Demand pricing.
- Requires 1 or 3-year commitment.
- Best for steady-state workloads.

## 4️⃣ Spot Instances
- Use unused AWS EC2 capacity.
- Up to **90% discount** compared to On-Demand.
- Can be interrupted with a 2-minute warning.
- Ideal for fault-tolerant and flexible workloads.

## 5️⃣ Dedicated Hosts
- Physical servers dedicated to your use.
- Suitable for compliance requirements or BYOL (Bring Your Own License).

## 6️⃣ Capacity Reservations
- Reserve compute capacity in a specific Availability Zone.
- Ensures capacity availability for any duration.
- Useful for critical workloads needing guaranteed resources.
