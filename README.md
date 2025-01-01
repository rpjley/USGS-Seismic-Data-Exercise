# USGS-Seismic-Data-Exercise
This repository contains a coding assignment for USGS-SAC-25-12553801-DE-RM, focused on processing and visualizing seismic data. Features include database design, waveform queries, metadata display, and interactive visualizations with maps and helicorder charts, showcasing skills in software development and geoscience data analysis.

## Features
- **Database Creation**: Initializes a database for seismic data and validates its structure with unit tests.
- **Seismic Data Visualization**: Generates interactive visualizations of seismic data, including helicorder plots and station maps.
- **Data Querying**: Supports querying seismic traces by station, time range, sampling rate, and location.

## Notebook Structure
The notebook is divided into the following sections:

### 1. Environment Setup
- **Purpose**: Installs and imports all necessary dependencies, including `ObsPy`, `Folium`, and `Matplotlib`.
- **Action**: Run all cells in this section to ensure the environment is ready for subsequent steps.

### 2. Database for Seismic Data
- **Purpose**: Sets up the SQLite database (`seismic_data.db`) and defines tables for storing station and waveform data.
- **Key Features**:
  - `Station` table stores metadata about seismic stations.
  - `WaveformTrace` table stores individual seismic traces and metadata.
- **Validation**: Includes unit tests to verify database setup and query functionality.

### 3. Visualization of Seismic Data
- **Purpose**: Contains functions for creating interactive and static visualizations of seismic data.
- **Features**:
  - `visualize_from_query`: Queries the database to pull applicable data.
  - `display_all`: Interactive tabbed layout for visualizing data by day.
  - `plot_helicorder`: Generates helicorder plots for seismic traces.
  - `create_map`: Creates interactive station maps with nearby station markers.
  - `create_metadata_chart`: Displays metadata for stations and traces.
- **Output**: Interactive visualizations and downloadable HTML files.

### 4. Main
- **Purpose**: Executes queries and integrates database and visualization functionalities.
- **Action**: Run this section to process data and generate visual outputs. Use the tabs and download buttons to explore the results.

---

## Prerequisites
- Python 3.8 or higher
- Required Packages:
  - `ObsPy`
  - `Folium`
  - `Matplotlib`
  - `SQLAlchemy`
  - `geopy`
  - `ipywidgets`

---

## How to Run
1. **Clone the Repository**:
   ```bash
   git clone <https://github.com/rpjley/USGS-Seismic-Data-Exercise.git>
   cd <USGS-Seismic-Data-Exercise>

2. **Upload Files**
 -Upload your .mseed files to the notebook environment (e.g., SEP01.mseed, SEP02.mseed).
 -Ensure the file paths in the Main section are updated to match your uploaded files.

3. **Open the Notebook**
 -Open the notebook in the intended environment

4. **Execute Sections Sequentially**
 - 1. Environment Setup
 - 2. Database for Seismic Data
 - 3. Visualization of Seismic Data
 - 4. Main Function

## Outputs
- Outputs
 - 1. Interactive Visualizations:
    - Tabs for exploring seismic data by day.
    - Meta Data Charts
    - Station Maps
    - Helicorder Plots
- 2. Downloadable HTML Files:
    - Each day's visualization can be downloaded using the provided buttons.

## Licenses:
    This project is licensed under the MIT License. You are free to use, modify, and distribute this software. See the LICENSE file for more details.

## Contact:

If you have any questions, feedback, or issues regarding this project, please feel free to reach out:

 - Name: Riley Johnson
 - Email: [\[rpjley@gmail.com\]](mailto:rpjley@gmail.com)
 - GitHub:  https://github.com/rpjley