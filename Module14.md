# Public Report

## Topic: Development of a Dashboard for Managing IT Security Indicators

## Objective

The purpose of this module was to develop a reliable and insightful dashboard for monitoring the IT security posture of the **ATVOS company**. The dashboard enables the tracking of critical indicators related to the security of devices and cloud resources, facilitating faster and more effective decision-making.

The dashboard covers three main areas:

### 1. Encrypted Devices with Active Antivirus

This sub-area ensures the protection of **endpoints**, meaning all computers (servers, notebooks, and desktops). The focus is on guaranteeing two essential layers of defense:

* **Active Antivirus:** Ensures that anti-malware protection software is installed, active, and updated on 100% of machines, preventing infections.
* **Disk Encryption:** Guarantees that the hard drive of devices (especially notebooks) is encrypted. If a device is lost or stolen, the data contained within it will be illegible to unauthorized persons, protecting the company's sensitive information.

### 2. Cloud Security

This sub-area monitors the security posture and compliance of the cloud environments used by the organization (such as **Azure, GCP, OCI, and O365**).

The main objective is to measure the **Compliance Score (CSPM)**, a score that evaluates the adherence of cloud environments to security best practices and internal policies. By continuously monitoring this score, the IT area can quickly identify and correct misconfigurations or vulnerabilities in the cloud environment, which is a growing vector for attacks.

### 3. LAPS Monitoring on Servers and Devices

**LAPS** (**Local Administrator Password Solution**) is a critical Microsoft tool focused on managing and securing the local administrator accounts on all Windows endpoints and servers.

The primary function of LAPS is to automatically rotate the password for these accounts periodically, securely storing it in the **Active Directory**. This prevents attackers from using the same local administrator password across multiple machines (**pass-the-hash**), significantly limiting **lateral movement** within the network after an initial compromise. The **% Active LAPS** indicator monitors whether this privileged password management solution is operational on all devices.

---

## Module 14 – IT Security Dashboard Development

### Sprint 1 – Planning

In this initial stage, we conducted project planning, which helped to gain a deep understanding of the most important steps.

### Sprint 2 – Persona and User Journeys

In this sprint, I was able to deeply understand the user's needs and perspectives.

We defined the visual concept and essential functionalities for the dashboard. **Mockups** and a **style guide** were created to serve as a visual foundation for the implementation in **Power BI**.

### Sprint 3 – Data Design and Prototyping

We defined the visual concept and essential functionalities for the dashboard. **Mockups** and a **style guide** were created to serve as a visual foundation for the implementation in **Power BI**. (Note: This text is a repeat of Sprint 2, which is maintained in the translation to reflect the original).

### Sprint 4 – Data Modeling

The data modeling for ATVOS's security indicators is centered on creating consolidated **fact tables**, optimized for Power BI, that transform raw data from operating systems and logs into monthly performance metrics. Specifically, Antivirus/Encryption data (source **SolarWinds**) and LAPS data (source **Active Directory**) are extracted at the machine level and, in the **ETL process**, aggregated to calculate the monthly coverage percentage relative to the total universe of active devices. The Cloud Security area, on the other hand, uses pre-aggregated (manual) score data at the Month and Platform level.

### Sprint 5 – Testing and Validation with Users

We conducted user interviews to validate the dashboard and ensure that the presented indicators met their needs. The final presentation was also delivered to the organization's partner.

---

## Future Improvements and Limitations

The primary goal of future improvements is to **increase indicator granularity**, allowing for more detailed and real-time tracking of security activities. Furthermore, we aim to detail the definition of the **Cloud Security Score (CSPM)**. This transparency is crucial for end-users to understand exactly which points of improvement should be prioritized to raise the Score, transforming the metric into an **actionable tool**.

## Conclusion

This project represents a fundamental step toward **data-driven management** in the IT area. By making indicators visible and accessible, it promotes team accountability, facilitates fault detection, and strengthens corrective and preventive planning.

In this module, the focus was on IT security, covering aspects such as **Encrypted and Antivirus-Enabled Devices, Cloud Security, and LAPS Monitoring on Servers and Devices**. The dashboard serves as a robust foundation for the final module, which will integrate dashboards from all sub-areas, delivering an executive and strategic view of IT performance across the entire organization.
