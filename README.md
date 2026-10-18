# 🚴 Fabric Bike-Station Monitoring Project

## 📌 Overview
An end-to-end **Microsoft Fabric Real-Time Intelligence** solution for bike-station monitoring.  
Live sample data is ingested into an Eventhouse via Eventstream, queried with KQL, visualized in a Real-Time Dashboard, and monitored with Activator alerts.  
The project is fully documented and published on GitHub with queries, screenshots, and architecture.

---

## 🏗️ Architecture
- **Eventstream**: Ingests live bike-station sample data  
- **Eventhouse (KQL DB)**: Stores streaming events in table `bikes`  
- **KQL Queries**: Latest status, empty/full stations, neighbourhood trends, time-series chart  
- **Real-Time Dashboard**: Map, charts, KPIs with auto-refresh  
- **Activator**: Email alerts when stations run out of bikes  
- **GitHub Repo**: Queries, screenshots, README  

---

## 📂 Source Data
Built-in Fabric sample dataset **“Bicycles”** with columns:  
- BikepointID, Street, Neighbourhood, Latitude, Longitude  
- No_Bikes, No_Empty_Docks  

---

## ⚙️ Steps Implemented
1. **Workspace Setup** → Created `bike-rti`  
2. **Eventhouse** → Created `bike_eh`  
3. **Eventstream** → Connected to Bicycles sample data  
4. **Table Creation** → Direct ingestion into `bikes` table  
5. **KQL Queries** → Latest status, empty/full stations, bikes by neighbourhood, trend line, map data, KPIs  
6. **Dashboard** → Map, bar chart, time chart, KPI cards, tables  
7. **Activator Alert** → Email notification when stations have 0 bikes  
8. **GitHub Repo** → README, queries, screenshots  

---

## 📊 Dashboard Highlights
- **Cards**: Empty stations count, Events in last 5 minutes  
- **Map**: Station locations sized by available bikes  
- **Bar Chart**: Bikes by neighbourhood  
- **Time Chart**: Bikes trend over last 30 minutes  
- **Tables**: Empty stations list, Full stations list  

---

## 🚀 How to Run
- Start Fabric trial and create workspace `bike-rti`  
- Create Eventhouse `bike_eh` and Eventstream `bike_stream`  
- Ingest Bicycles sample data into table `bikes`  
- Run KQL queries in Queryset `bike_queries`  
- Build Real-Time Dashboard `bike_dashboard`  
- Configure Activator alert `bike_alerts`  

---

## 💡 Interview Pitch
*"I built a real-time streaming project in Microsoft Fabric: bike-station events flow into Eventstream and Eventhouse, queried with KQL, visualized in a live dashboard, and monitored with Activator alerts. I used Fabric’s built-in sample data, but the same pipeline works with custom producers or IoT sources."*

---

## 📍 Author
👨‍💻 **Suresh Gadi**  
Azure Fabric Data Engineer | Hyderabad, India
