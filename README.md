# Predicting-Used-Car-Price

[Dataset]( https://aws.amazon.com/marketplace/pp/prodview-y77x3t6zisn4w?sr=0-2&ref_=beagle&applicationId=AWSMPContessa) <br>

## Summary
* **44,365** total car sales for Carvana in Aug 2022
* **88.48%** accuracy estimating sold price

## Code & Resources Used
**JupyterLab:** 3.3.3 <br>
**Python within JupyterLab:** 3 <br>
**Packages:** pandas, numpy, matplotlib, seaborn, sklearn <br>
**Articles/Code:**
   - [Used Car Modeling]( https://towardsdatascience.com/end-to-end-data-science-project-predicting-used-car-prices-using-regression-1b12386c69c8)

## Exploratory Data Analysis
We initially looked at our basic colum structures looked at numerical column stats
The dataset was very clean with no NaNs
* Median Year of cars sold - 2016
* Year range of cars sold - 2009-2013
* Median Miles of cars sold - 52,744
* Miles range of cars sold - zero to 115,875
* Median Sold Price - $25,273
* Range of Sold Price - $8,990 to $129,990
<img style="display: inline; margin: 0 5px;" title="Descriptive Stats" src="img/Dataset descriptive stats.png" alt="" width="800" height="300"/>

