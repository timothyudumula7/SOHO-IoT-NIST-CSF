# SOHO-IoT-NIST-CSF
SOHO IoT Cybersecurity Framework (NIST CSF-Based)
Author: Timothy Udumula
Course: CYBR 624 – Cybersecurity Project
Institution: University of Maryland, Baltimore County
Instructor: Dr. Behnam Shariati

📄 Section 1: Introduction and Problem Statement
This project explores the security vulnerabilities of Internet of Things (IoT) devices in Small Office/Home Office (SOHO) environments. While IoT offers usability and efficiency, it also introduces significant risk due to:

Weak built-in security

Insecure communication protocols (e.g., HTTP, ARP)

Lack of firmware updates

Limited access control

The project focuses on building a policy-driven, technical solution to secure SOHO networks using network segmentation, access control, and automated update mechanisms aligned with the NIST Cybersecurity Framework (CSF).

🔍 Research Question:
How can we implement a lightweight, policy-driven technical solution for SOHO IoT security using principles of network segmentation, zero trust, and automation?

📚 Section 2: Literature Review
This section evaluates existing research on IoT security challenges and solutions, including:

Insecure network protocols and on-path attacks (Okereke et al., 2024)

Firmware vulnerabilities and lack of OTA updates (Kabir et al., 2023; Zhao et al., 2022)

The need for readable, enforceable security policies in SOHO networks (Alkhurayyif & Weir, 2017)

Key insights:

IoT security frameworks often lack practicality in SOHO contexts.

Access control and DNS monitoring are recurring themes for mitigation.

Most existing solutions do not consider readability or scalability in small environments.

🛠️ Section 3: Methodology and Implementation
The final section details the technical and policy solution, centered on the NIST CSF (v2.0) framework. The solution is tested in a SOHO setup and includes:

🔧 Technical Implementations:
VLAN Segmentation:
VLAN10 (Admin), VLAN20 (Users), VLAN30 (IoT), VLAN40 (Backup)

Access Control Lists (ACLs):
Restrict inter-VLAN traffic; allow Admin-only elevated access

DNS Filtering via Pi-hole:
Real-time query filtering and logging for all VLANs

Automatic Updates:
Cron job–based update mechanism to reduce manual maintenance

🧱 Policy-driven Model:
Aligned with NIST CSF core functions: Identify, Protect, Detect, Respond, Recover

Built with zero-trust principles

Designed to be scalable, lightweight, and easy to implement for SOHO users of varying technical ability

✅ Results:
Improved DNS visibility and control

Reduced lateral movement and botnet exposure

Less reliance on manual updates

Clear, enforceable security policy for small networks

