---
title: "VEIN model"
author: "Sergio Ibarra-Espinosa"
date: "22 de abril de 2017"
output: html_document
---



[![Travis-CI Build Status](https://travis-ci.org/ibarraespinosa/vein.svg?branch=master)](https://travis-ci.org/ibarraespinosa/vein)
[![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/github/ibarraespinosa/vein?branch=master&svg=true)](https://ci.appveyor.com/project/ibarraespinosa/vein)
[![](http://cranlogs.r-pkg.org/badges/vein)](http://cran.rstudio.com/web/packages/vein/index.html)
[![Rdoc](http://www.rdocumentation.org/badges/version/vein)](http://www.rdocumentation.org/packages/vein)



![](p2.png)

## Vein Package

**V**ehicular **E**missions **IN**ventory **(VEIN)** model.  



Read the DESCRIPTION file. You need several packages to run **vein**.

- [sp](https://github.com/edzer/sp/) 
- [units](https://github.com/edzer/units/) 
- [raster](http://cran.r-project.org/package=raster)
- [rgdal](https://github.com/cran/rgdal)
- [rgeos](https://github.com/cran/rgeos)

Also, if you want to properly run the demo, install these packages:

- ggplot2
- RColorBrewer


```r
# 0.2.2-25
library(devtools)
install_github("ibarraespinosa/vein")
library(vein)
demo(VEIN)
```

or


```r
# 0.2.2-3
install.packages("vein")
library(vein)
```



I've created the following classes:

- Vehicles (1/h) 
- Speed  (km/h)
- EmissionFactors (g/km)
- EmissionFactorsList (g/km)
- Emissions  (g/h)
- EmissionsArray  (g/h)
- EmissionsList  (g/h)
- Evaporative  (g/d)

Each class has the methods print, plot and summary.

New information will also be added to the documentation of emission factors.

If you encounter any issues while using VEIN, please submit your issues to: https://github.com/ibarraespinosa/vein/issues/

If you have any suggestions just let me know to zergioibarra@gmail.com

Thanks and enjoy VEIN!

### **Roadmap** (not in order)

- 0.3: Migrate to [sf](https://github.com/edzer/sfr/)
- 0.4: **Estimator** structured folders and scripts???
- 0.5: Graphical interface (probably similar [MODIStsp](https://github.com/lbusett/MODIStsp))
- Improve vehicle classification (all vehicle includes engine size)
- Estimation of evaporative emissions with Copert Tier 3
- More speciations
- Topdown estimation