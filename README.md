# 🧭 MSP-out  
**Exploratory Data Analysis of European Maritime Spatial Plans**

---

## 📘 Overview
**MSP-out** (Maritime Spatial Planning Output Data analytical module) is a tool designed to perform **exploratory data analysis (EDA)** on the spatial representations of **European Union Maritime Spatial Plans (MSPs)**.  

It supports planners and decision-makers in:
- Summarizing the main characteristics of MSPs  
- Identifying spatial patterns  
- Comparing plans across scales (national, transnational, sea-basin, and EU-wide)  
- Supporting revision and update phases of maritime spatial planning

---

![image](https://github.com/user-attachments/assets/a7dfb627-f373-4856-9908-27c821d76c28)


## 🌍 Data Sources
The tool integrates authoritative European geospatial data sources such as:
- [**EMODnet Human Activities**](https://emodnet.ec.europa.eu/en/human-activities)
- [**EMSA**](https://emsa.europa.eu/)

Data are accessed through **interoperable WFS/WMS services**, ensuring **harmonization** and **interoperability** across different national datasets.  

In addition to official EMODnet MSP datasets, **draft or non-published plans** can also be analysed — provided they are structured according to the **standard EMODnet MSP data model** (European Commission, 2021). Users can request data integration through the tool administrators.

---

## 🧩 Architecture
MSP-out is implemented as an **interactive web application** using **[Streamlit](https://streamlit.io/)** and follows a **modular architecture** separating:
- Data preprocessing  
- Spatial and statistical analysis  
- Interactive visualization  

The tool is **containerized** for reproducibility and easy deployment (Docker-ready).

---

## ⚙️ Technology Stack

| Component | Description |
|------------|-------------|
| **Python** | Core programming language |
| **Streamlit** | Framework for building interactive web applications |
| **pandas / geopandas** | Data manipulation and geospatial operations |
| **shapely** | Geometry validation and topology correction |
| **folium** | Interactive map visualization (Leaflet.js integration) |
| **plotly, matplotlib, seaborn** | Interactive and static plotting libraries |
| **rasterstats** | Spatial summaries linking raster and vector data |
| **pyarrow, fastparquet** | Efficient I/O with Parquet datasets |

---

## 📊 Analyses and Outputs
MSP-out provides several types of analyses, including:
- **Zoning Elements analysis** – count, coverage, and disjoint index  
- **Sea Uses** – distribution and spatial coverage of activities  
- **Sea Use & Function** – regulatory framework analysis  
- **Coexistence analysis** – overlap of maritime uses (UpSet plots)  
- **Diagnosis** – comparison of original plan attributes vs EMODnet model (Sankey, Treemap)

### Output formats:
- Interactive maps and charts  
- Downloadable figures (PNG)  
- Tabular results (CSV)  
- Option to **publish analyses** as permanent interactive web pages  

---

## 🚀 Deployment & Access
- **Online version (v0.11):**  
  🔗 [https://geoapps.tools4msp.eu/ReMAP_MSP_out](https://geoapps.tools4msp.eu/ReMAP_MSP_out)

- **Source code:**  
  🔗 [https://github.com/EMFAF-ReMAP/MSP-out](https://github.com/EMFAF-ReMAP/MSP-out)


## 👥 Contributors
- Stefano Menegon
- Sara Sottoriva
- Alessandro Sarretta
- Luca Fucci
- Alessandro Mulazzani

