
R-to-Python Table
=======================

Commands
^^^^^^^^^

=========== ================ =======================
R           Python           Notes
=========== ================ =======================

library()   import

lapply()    map

ddplyr      apply (`pandas`)

lm          ols (`statsmodels`)


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
