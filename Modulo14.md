# PublicReport

*Theme:* Dashboard Development for IT Infrastructure Indicator Management

---

### *Objective*

The goal of this module was to develop a consolidated and informative dashboard for monitoring the organization’s IT infrastructure. The dashboard provides a real-time view of critical indicators related to *security, **availability, and **system performance*, enabling faster and more effective decision-making.

The dashboard covers four main areas:

* *Firewall:* Monitors the number of days without instability, the main attack reasons, and threat levels (low, medium, high).
* *Network:* Analyzes the causes of network instability and the corresponding downtime impact.
* *PIMS System:* Displays current availability status, uptime percentage, total downtime, and mean time to recovery.
* *4G Network:* Shows incident counts by unit, average latency, and download speed.

Additionally, the dashboard is structured using a *star schema dimensional model*, which allows integrated analysis across different infrastructure domains.

---

## *Module 14 – IT Infrastructure Dashboard Development*

### *Sprint 1 – Planning and Personas*

In this initial stage, we carried out project planning and developed *Personas and User Journeys*, which helped us understand the user profiles and their monitoring needs in depth.

### *Sprint 2 – Design and Prototyping*

We defined the visual concept and essential functionalities for the dashboard. *Mockups and a style guide* were created to serve as the visual foundation for the Power BI implementation.

### *Sprint 3 – Data Modeling*

A *star schema* data architecture was developed, consisting of one fact table (Monitoramento_TI) and four dimension tables (Dim_Firewall, Dim_Rede, Dim_PIMS, Dim_4G). The model was built based on manually extracted data from Grafana in CSV format, later transformed and modeled in Power BI.

### *Sprint 4 – Dashboard Construction*

With the data structure in place, we built the dashboard in Power BI. This involved data modeling, importing extracted Grafana data, and performing transformations using Power Query.

### *Sprint 5 – User Testing and Validation*

We conducted *user interviews* to validate the dashboard and ensure the presented indicators met their needs. The final presentation was also delivered to the organization’s partner.

---

## *Future Improvements and Limitations*

The main improvement identified is the *automation of data ingestion* through direct integration with the *Grafana API* or its database. Currently, data is manually imported via CSV files, which limits real-time updates and increases operational workload.

---

## *Conclusion*

This project represents a key step toward *data-driven management* in the IT area. By making *indicators visible and accessible*, it promotes team accountability, facilitates failure detection, and strengthens corrective and preventive planning.

In this module, the focus was on *IT infrastructure, covering aspects such as **system availability, network stability, and mobile connectivity performance. The dashboard serves as a strong foundation for the final module, which will integrate dashboards from all sub-areas, delivering an **executive and strategic overview* of IT performance across the organization.
