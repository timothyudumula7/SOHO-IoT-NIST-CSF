SOHO IoT Cybersecurity Framework (NIST CSF-Based)

**Author:** Timothy Udumula  
**Course:** CYBR 624 – Cybersecurity Project  
**Institution:** University of Maryland, Baltimore County  
**Instructor:** Dr. Behnam Shariati

---

## 🔷 **Section 1: Introduction and Problem Statement**

This project explores the security vulnerabilities of Internet of Things (IoT) devices in **Small Office/Home Office (SOHO)** environments. While IoT offers usability and efficiency, it also introduces significant risks due to:
- Weak built-in security  
- Insecure communication protocols  
- Lack of firmware updates  
- Limited access control  

The project focuses on building a **policy-driven, technical solution** to secure SOHO networks using:
- Network segmentation  
- Access control  
- Automated update mechanisms  

All solutions are aligned with the **NIST Cybersecurity Framework (CSF)**.

### **🔍 *Research Question***
*How can we implement a lightweight, policy-driven technical solution for SOHO IoT security using principles of network segmentation, zero trust, and automation?*

---

## 🔷 **Section 2: Literature Review**

This section evaluates existing research on IoT security challenges and solutions, including:
- Insecure protocols and attack surfaces  
- Firmware update limitations  
- Complexity and readability issues in security policy  
- Gaps in scalability for small-scale (SOHO) environments  

**Key insights:**
- Existing frameworks often lack SOHO applicability  
- Network-level protections (e.g., ACLs, DNS logging) are essential  
- Human-readable and low-overhead policies are vital for adoption  

---

## 🔷 **Section 3: Methodology and Implementation**

This section details the technical and policy solutions tested in a SOHO lab setup and built upon the **NIST CSF v2.0** core functions.

### ***🔧 Technical Implementations***
- **VLAN Segmentation:**  
  VLAN10 (Admin), VLAN20 (Users), VLAN30 (IoT), VLAN40 (Backups)  
- **Access Control Lists (ACLs):**  
  Limits lateral traffic and enforces least-privilege access  
- **DNS Filtering (Pi-hole):**  
  Logs and filters DNS requests to detect malicious domains  
- **Automatic Updates:**  
  Cron job–based automation for firmware and OS patching  

### ***📐 Policy Model***
- Based on **NIST CSF**: Identify, Protect, Detect, Respond, Recover  
- Applies **zero-trust** principles  
- Designed for low-maintenance, SOHO-scale environments  

---

## ✅ **Outcomes**
- Reduced lateral movement and botnet exposure  
- Minimized manual update burden  
- Enforced scalable and enforceable security policy for SOHO networks  

---

📎 *Please find the full project PDFs in the repository if applicable.*

🙏 Thank you for your time!
