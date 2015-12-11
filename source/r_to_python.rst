
R-to-Python Table
=======================

*Note this section is still very preliminary. Please check back for updates.* 

If you know of any existing sources for this type of table, `please send me an email letting me know! <mailto:nickeubank+pss@gmail.com>`_

Outside Sources
^^^^^^^^^^^^^^^^

`A nice table of pandas-to-R translations. <https://dato.com/learn/translator/>`_

Commands
^^^^^^^^^


=========== =================== =======================
R           Python              Notes
=========== =================== =======================
library()   import
lapply()    map
ddplyr      apply (`pandas`)
lm          ols (`statsmodels`) 
=========== =================== =======================


Libraries
^^^^^^^^^

=========== =================== ============================
R           Python              Notes
=========== =================== ============================
ggplot      seaborn
rgdal       geopandas / fiona / fiona and rasterio are 
            rasterio            embedded in GeoPandas
sp          geopandas / shapely GeoPandas builds off shapely
rgeos       geopandas / shapely GeoPandas builds off shapely
=========== =================== ============================
