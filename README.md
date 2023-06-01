**SCL Data - Data Ecosystem Working Group**


<center>
<p float="left">
  <img src="https://scldata.iadb.org/assets/iadb-7779368a000004449beca0d4fc6f116cc0617572d549edf2ae491e9a17f63778.png" width="17%" style="margin:50px 50px">
</p>
</center>

<h1 align="center"> Spatial Connectivity  </h1>


## Index:
--- 
- [Description and Context](#description-and-context)
- [Structure](#structure)
- [Methodology](#methodology)
- [Next Steps](#next-steps)
- [Author(s)](#authors)

## Description and Context
---

This Python script takes geospatial data in the form of shapefiles and tile data to perform connectivity analysis. It performs spatial joins, data conversions, and statistical analysis, providing insights into average download and upload speeds for the Latin America and the Caribbean Region. The output can be saved in CSV format or visualized as plots. This script is useful for studying connectivity trends and patterns in various geographic regions.

The script is designed to be used in an AWS environment and expects certain environment variables and input files to be available in specific locations. The data sources used include Ookla OpenData and local geospatial basemaps.


## Structure
---

The script is divided into several sections:

1. Environment setup: Loading of environment variables and import of necessary Python libraries.

2. Data loading: Retrieval of shapefile data and tile URLs.

3. Data preprocessing: Conversion of data units and spatial joining of tile and shapefile data.

4. Statistical analysis: Computation of weighted averages for download and upload speeds.

5. Data output: Saving of processed data in CSV format.

6. Visualization: Creation of plots for download speeds at different administrative levels.


## Methodology
---

The script uses the GeoPandas library to perform spatial joins between the tile data and the shapefiles for administrative levels 1 and 2. This allows the connectivity data to be linked with geographic regions.

After joining the data, it computes the weighted averages for download and upload speeds based on the number of tests conducted. The results are saved as CSV files.

Finally, it creates plots to visualize download speeds at different administrative levels. The plots are saved as JPEG images.

<center>
<img src="./speed_lac_municipality.jpg" width="500">
</center>

## Next steps 
---



### Authors
- [María Reyes Retana](https://github.com/mariarrt94)

We would like to express our gratitude to [Ookla](https://www.ookla.com/) for making their Open Data available. This project uses data and is based on [Ookla Open Data](https://github.com/teamookla/ookla-open-data) repository. The data used includes tile data that provide valuable insights into global connectivity trends.

The raw data, its structure, and collection methodology can be found in the [Ookla Open Data repository](https://github.com/teamookla/ookla-open-data) on GitHub. All rights concerning the Ookla data belong to Ookla.






