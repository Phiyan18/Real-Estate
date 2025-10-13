# 🏙️ SkyLine GrowthTracker
<img width="720" height="720" alt="Gemini_Generated_Image_oyf6m5oyf6m5oyf6" src="https://github.com/user-attachments/assets/0b3ba9d9-c38c-4263-9167-1792a29035ca" />

**SkyLine GrowthTracker** is a geospatial analytics project that leverages **Google Earth Engine (GEE)** and **Python** to monitor, analyze, and visualize **urban growth patterns**.  
It detects and tracks recent building developments, providing insights into city expansion and construction dynamics over time.

---

## 🌟 Overview

Urban growth is a key indicator of socioeconomic development — and with increasing satellite data availability, it's now possible to monitor it more effectively.  
SkyLine GrowthTracker simplifies this process by using Google Earth Engine’s satellite imagery and geospatial datasets to:

- Detect newly built-up areas within a region.
- Convert Earth Engine feature collections to GeoDataFrames.
- Generate visualizations that highlight spatial growth patterns.
- Provide both statistical and geospatial insights into urban development.

---

## 🚀 Features

- 🌍 **Satellite-based urban analysis** with Google Earth Engine  
- 🏗️ **Building footprint extraction** from high-resolution imagery  
- 🗺️ **Interactive geospatial mapping** using Folium and Geemap  
- 📊 **Data analytics and visualization** with Pandas, Matplotlib, and Seaborn  
- ⚡ **Efficient workflows** with GeoPandas and TQDM for progress tracking  
- 💾 **Export-ready GeoData** (Shapefile, GeoJSON, CSV)

---

## 🧰 Tech Stack

| Category | Tools |
|-----------|--------|
| **Core** | Python 3.9+, Google Earth Engine |
| **Visualization** | Folium, Geemap, Matplotlib, Seaborn |
| **Data Handling** | Pandas, NumPy, GeoPandas |
| **Geometry Processing** | Shapely |
| **Progress Monitoring** | TQDM |

---

## 📦 Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/SkyLine_GrowthTracker.git
cd SkyLine_GrowthTracker
```

### 2️⃣ Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate      # Linux / macOS
venv\Scripts\activate         # Windows
```

### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Authenticate with Google Earth Engine
```bash
earthengine authenticate
```

---

## 🧠 Usage

### Run the Jupyter Notebook
```bash
jupyter notebook SkyLine_GrowthTracker.ipynb
```

### Example Workflow
1. Define your **region of interest (ROI)** (can be a polygon or uploaded shapefile).
2. Run the cells sequentially to:
   - Retrieve recent building footprints.
   - Convert Earth Engine features to a GeoDataFrame.
   - Visualize results and export data.

```python
import ee
from SkyLine_GrowthTracker import get_recent_buildings, ee_fc_to_gdf

ee.Initialize()
roi = ee.Geometry.Polygon([...])

buildings = get_recent_buildings(roi)
gdf = ee_fc_to_gdf(buildings)
gdf.head()
```

3. View **interactive maps** and **visual analytics** within the notebook.

---

## 📈 Example Outputs

### 🗺️ Geospatial Visualization
Interactive **Folium** maps show the distribution and density of new buildings in the region.

### 📊 Analytical Charts
Graphs generated with **Matplotlib** and **Seaborn** illustrate:
- New building counts by year or region  
- Area expansion rates  
- Growth intensity heatmaps  

> *(Add screenshots or map previews here — e.g. `images/map_preview.png`)*

---

## 📁 Project Structure

```
SkyLine_GrowthTracker/
├── SkyLine_GrowthTracker.ipynb   # Main Jupyter Notebook
├── data/                         # Input / output spatial data
├── images/                       # Visualization outputs (optional)
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation
```

---

## 🧑‍💻 Author

**Phiyan**  
Engineering Student & Geospatial Enthusiast  
📧 *Contact:* (optional – add email or LinkedIn if you wish)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 💡 Future Improvements

- 🛰️ Time-lapse visualization of urban expansion  
- 🤖 Integration with AI-based building classification models  
- 🌆 Automated multi-region comparison and dashboard view  
- 📦 Web-based deployment using Streamlit or Dash  

---

## 🤝 Contributing

Contributions are welcome!  
1. Fork the repository  
2. Create a new branch  
3. Commit changes  
4. Open a pull request  

---

## 🙌 Acknowledgments

- [Google Earth Engine](https://earthengine.google.com/) for geospatial data and APIs  
- [Geemap](https://geemap.org/) for bridging Earth Engine and Python visualization  
- [GeoPandas](https://geopandas.org/) and [Shapely](https://shapely.readthedocs.io/) for spatial analysis  
- [Folium](https://python-visualization.github.io/folium/) for map rendering  

---

### 🌐 “Mapping the growth of tomorrow, today.”
