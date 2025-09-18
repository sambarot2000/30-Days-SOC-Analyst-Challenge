# Day 02 — Understanding the ELK Stack

## Objective
Learn about the **ELK Stack** — Elasticsearch, Logstash, and Kibana — which is essential for **log collection, analysis, visualization, and alerting** in a SOC environment.

---

## What is ELK?

The **ELK Stack** is a set of open-source tools used for **centralized logging and security analytics**:

1. **Elasticsearch**  
   - A distributed search and analytics engine.  
   - Stores and indexes logs for **fast searching and querying**.  
   - Can handle both structured and unstructured data.  
   - **SOC use:** Quickly search and analyze security events across endpoints and servers.

2. **Logstash**  
   - A pipeline tool that collects data from multiple sources, **processes it**, and sends it to Elasticsearch.  
   - Supports input, filter, and output plugins for data normalization.  
   - **SOC use:** Collect logs from Windows, Linux, and network devices, then forward them to Elasticsearch.

3. **Kibana**  
   - A visualization and analytics tool for Elasticsearch data.  
   - Lets you create **dashboards, charts, and reports**.  
   - **SOC use:** Monitor security events, investigate incidents, and track trends visually.

> Together, the ELK Stack works as follows:  
> **Logstash collects and processes logs → Elasticsearch stores and indexes → Kibana visualizes and monitors.**

---

## Why ELK is Important for SOC

| Feature | Benefit for SOC Analysts |
|---------|-------------------------|
| Centralized Logging | Access all logs in one location |
| Real-Time Monitoring | Detect threats immediately |
| Correlation & Search | Identify patterns across large datasets |
| Dashboards & Alerts | Track incidents and create alerts |
| Scalability | Supports growth in infrastructure and data |

---

## Components to Deploy

- **ELK Stack:** Elasticsearch, Logstash, Kibana  
- **Beats Agents:**  
  - Winlogbeat for Windows logs  
  - Filebeat for Linux and application logs  
- **Alerting Tools:** Elastic Watcher or third-party integrations  
- **Lab Servers:** Windows, Linux, and Fleet servers for log collection

---

## Outcome

By completing this step, you will:  
- Understand the **ELK architecture**  
- Be ready to configure your SOC lab  
- Begin ingesting logs, visualizing data, and creating dashboards

---

> **Tip:** Start small by collecting logs from a few endpoints. Gradually expand as you become comfortable with ELK.
