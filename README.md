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
We initially looked at our basic colum structures looked at numerical column stats.  The dataset was very clean with no NaNs.
* Median Year of cars sold - 2016
* Year range of cars sold - 2009-2013
* Median Miles of cars sold - 52,744
* Miles range of cars sold - zero to 115,875
* Median Sold Price - $25,273
* Range of Sold Price - $8,990 to $129,990
<img style="display: inline; margin: 0 5px;" title="Descriptive Stats" src="Images/Dataset descriptive stats.png" alt="" width="800" height="300"/>

We also looked for any miles vs sold price outliers
* There were 5 outliers with miles greater then 110,000 miles and when exploring the data 2 used vehicles with 0 miles, we removed these
* We kept the higher priced cars as there was no real good dividing line
<img style="display: inline; margin: 0 5px;" title="Miles vs Price" src="Images/Miles vs Price.png" alt="" width="800" height="300"/>

**Data Wrangling**

With only 13 columns, it was easy to decipher what we wanted to keep and remove
The next step as to recode categorical data into numerical so we could run a correlation matrix
* We used 2 methods for recoding categorical data
   * For car model, we used a standard recode method, creating a new numerical column
   * For make and trim, since there were so many different variables, we used Label Encoding

Next we ran a Correlation Matrix
* There is high correlation for sold price between year and miles.  Which in the real world makes sense.
<img style="display: inline; margin: 0 5px;" title="Correlation Matrix" src="Images/Correlation Matrix.png" alt="" width="800" height="300"/>
