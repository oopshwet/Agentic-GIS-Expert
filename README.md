🌍 Agentic GIS Expert

An open-source Chain-of-Thought powered multi-agent system that turns natural language queries into complete geospatial analysis workflows.

Built for disaster response, planning, and spatial decision-making — with seamless integration with ISRO’s platforms like BHUVAN, Bhoonidhi, and VEDAS.





✨ Key Features

🧠 Natural Language to GIS Pipeline via Chain-of-Thought
🤖 Multi-agent system with planner, data, analysis & map agents
🗺️ Interactive maps (Folium / Leaflet)
🗂️ Works with shapefiles, GeoTIFFs, satellite & climate data
📦 Integration-ready with ISRO’s Bhuvan, Bhoonidhi, VEDAS
📊 Transparent, reproducible, and shareable workflows
🧪 Example Query

“Identify flood-prone areas in Odisha with low elevation and high rainfall over 3 years.”
🧠 Chain-of-Thought Breakdown:

Load Odisha boundary layer
Fetch flood-prone zones from BHUVAN
Apply DEM raster to mask elevation < 50m
Fetch 3-year rainfall data from Bhoonidhi
Intersect all layers & generate summary
Visualize results on map + write report
🚀 Demo

Coming Soon: Hosted Streamlit demo link
To run locally: see Setup below.

📁 Project Structure

agentic-gis-expert/
│
├── agents/ → Agent definitions (planner, map, data, etc.)
├── tools/ → GIS tool functions (buffer, intersect, etc.)
├── workflows/ → Sample workflows and query plans
├── data/ → Sample shapefiles, GeoTIFFs
├── ui/ → Streamlit or React frontend
├── docs/ → Markdown documentation (detailed usage, APIs)
├── app.py → Entry point (backend + agent engine)
├── requirements.txt → Python dependencies
└── README.md → This file

🛠️ Tech Stack

Layer	Tools/Frameworks
LLM / Reasoning	OpenAI GPT-4, LangChain, AutoGen (optional)
GIS Processing	GeoPandas, Shapely, Rasterio, PostGIS
Agent Framework	LangChain Agents / CrewAI
Data Handling	GDAL, Pyproj, Pandas
UI Frontend	Streamlit / React + Leaflet.js
Map Viewer	Folium, MapLibre, Kepler.gl
Deployment	Docker, Render / HuggingFace Spaces
