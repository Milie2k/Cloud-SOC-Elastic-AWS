# ☁️ Cloud-Based SOC Deployment (Elastic SIEM & AWS)
**Capstone Project - AltSchool Africa**

## 📌 Project Overview
This project involved the end-to-end deployment of a functional **Security Operations Center (SOC)** in a cloud-native environment. By integrating **Elastic SIEM** with **AWS telemetry**, I established comprehensive visibility into identity (IAM), network (VPC Flow Logs), and host-level activities.

## 🛠️ Architecture & Stack
- **SIEM Platform:** Elastic Cloud (Elasticsearch, Kibana)
- **Cloud Infrastructure:** AWS (EC2, S3, VPC, CloudTrail)
- **Log Sources:** - **AWS CloudTrail:** For monitoring API calls and IAM activity.
  - **VPC Flow Logs:** For network traffic analysis.
  - **Elastic Agents:** Installed on EC2 instances for host-level telemetry.
- **Integrations:** AlienVault OTX (Open Threat Exchange) for threat intelligence.

## 🚀 Key Accomplishments
1. **Infrastructure as Security:** Deployed EC2 instances in `eu-north-1` and configured S3 buckets as centralized destinations for VPC Flow Logs.
2. **Detection Engineering:**
   - Implemented Out-of-the-box (OOTB) rules for cloud threat detection.
   - Created a **Custom SSH Activity Rule** to alert on unauthorized remote access attempts.
3. **Attack Simulation & Validation:**
   - Simulated unauthorized IAM user/group creation to verify CloudTrail alerting.
   - Performed network "ping" tests and SSH brute-force simulations to validate VPC flow monitoring.
4. **Endpoint Forensics:** Analyzed a Windows EC2 instance using Event Viewer to identify **Event ID 1102** (Audit Log Cleared), a common indicator of log tampering by attackers.

## 🔍 Incident Triage Workflow
- **Alert Generation:** Detection of suspicious IAM activity.
- **Investigation:** Correlated CloudTrail events with EC2 host logs.
- **Documentation:** Documented findings and response actions in a technical incident report.

## 📊 Visual Proof
*(Full Capstone Report and Architecture Diagrams included in the repository)*
