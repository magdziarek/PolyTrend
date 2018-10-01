PolyTrend is a change detection algorithm developed by Dr Sadegh Jamali at Lund University. It works on pixel-level time-series and classifies trends in vegetation into linear, quadratic, cubic, concealed and no-trend types.

For details read: PolyTrend: Jamali, S.; Seaquist, J.; Eklundh, L.; Ardö, J. (2014): Automated mapping of vegetation trends with polynomials using NDVI imagery over the Sahel. In Remote Sensing of Environment 141, pp. 79–89. DOI: 10.1016/j.rse.2013.10.019

To use the scripts here you will need to install Anaconda and Jupyter Notebook first (see SettingUpJupyterNotebook.pdf) and download a relevant script. 

List of scripts:
- Change_detection_PolyTrend script is the longest: it reduces large image collections to annual NDVI values, using either the maximum or the mean value of NDVI for each year, then splits the images into pixel time-series and applies PolyTrend
- PolyTrend is the algorithm that fits polynomials into pixel-level data and does nothing more. You will need your own data in the form of a list of values, minimum 4 values (to fit the cubic polynomial), eg. [0.789, 0.756, 0.755, 0.746]

If you prefer to use your own data, the algorithm is also available in: 
- Matlab, 
- as a package in RStudio: https://cran.r-project.org/web/packages/PolyTrend/index.html 
- as a webtool: http://polytrend.gis.lu.se/
