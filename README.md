# Programming-for-Data-Analytics-Project-Autumn-2019

![car-reg](Images/car-reg.png)


## Scope
To simulate a dataset for a real life phenomenon that accurately reflects the values, distributions and relationships of a real dataset for the same phenomenon. 
[See here for instructions](/ProgDA_Project.pdf)

## Desciption
The data created in this repository is to simulate the sales of hybrid and electric cars in Dublin and and it's commuter counties for 2019 to date. This data is of interest to the author, who is considering a hybrid or full electric cars for the next car purchase. Viewing trends and data related to sales of such vehicles in and close to Dublin will be of relevance. 

The main body of work in this assignment is performed in a jupyter notebook. If viewing through Github, the ipynb file is best viewed through nbviewer, as certain text formatting will not load correctly when viewing through GitHub. Please follow the below link to view the notebook in nbviewer  [Create a Data Set Project jupyter notebook](https://nbviewer.jupyter.org/github/BarryClarke/Create-a-Data-set-Project-Autumn-2019/blob/master/New%20Electric%20car%20sales.ipynb) 

To view the source code in jupyter notebook, please follow the below instructions:
1. In this repoistory (ie Create-a-Data-set-Project-Autumn-2019) click on the clone or download button and copy the URL ![clone](Images/Clone.PNG)
2. In cmder/command prompt on your system clone the repository using the command git clone followed by paste the URL
3. Go to the directory where you saved cloned the Repository
4. Type "jupyter notebook" for the repository to open in jupyter
5. When Jupyter notebook opens, click on the numpy.random package.ipynb file
6. In this file, locate the *Kernal* tab and select *Restart & Run All* <br>
**Note:** This assumes you have python and Github setup on your machine.<br>
 
The final simulated dataset consists of 1000 data points for 10 variables:
1. **Model:** The make of car
2. **Make:** The manufacturer of the car 
3. **Classification:** The class of car 
4. **Technology** The engine type
5. **Price** The price of the car
6. **Range** The range/distance that can be travelled when powered on battery
7. **Month** The Month the car was registered
8. **Location** County where the car is registered (Only Dublin and it's commuter counties)
9. **Colour** The colour of the car
10. **Price per Month** Including loan intereste rates, the prcie of the car per month, based on a 7 year payback period

In simulating this particular dataset, almost all of the data was categorical ie. a finite number of options were available within each variable. This just happened to be the nature of this particular dataset and topic chosen, which proved slightly frustrating as it offered limited scope to examine and use the many different distributions offered by the numpy.random package. With that said, for this particular dataset, all necessary variables for the author were explored and simulated using what is believed to be the correct and most efficient code. 

Background research on hybrid and Electric car sales in Ireland for 2019 found statistical summaries for car sales numbers for **Model**, **Location**, **Month** and **Colour**. Using these statistics with the numpy.random.choice() function yielded simulated data that was shown to be accurate to researched recorded data.
For some of the variables (**Make**, **Cassification**, **Technology**, **Price** and **Range**) there was a direct relationship with the Model of car. In simulating these columns, _for_ and _if_ loops were utilised to generate the correct data corresponding to each Model.
In dealing with the **Price** of each data point simulated, the numpy.random.normal() function was applied to simulate the small price deviations between sales of the same car model from different dealerships.

Finally, in calculating the preice per month of a loan taken out for an assumed 7 years, the numpy.random.uniform() function was used to simulate the varying interest rates across all lending instiutions.

All research, code and verification of simulated data is contained within the _New Electric car sales.ipynb_ jupyter notebook file contained within this respoitory, along with all References used.




