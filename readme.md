# <p align='center'>IT496 - Introduction to Data Mining</p>
**Course Project**: 1 <br/>
**Lab Group**: T06<br />
**Dataset**: EV Charging Station


## **Introduction**
The Electric Vechilce(EV) Charging station dataset provides the information about the usage patterns of EV Charging stations in the city of Palo Alto, California. This includes data of the time from July 2011 to Jan 2021. It is an open dataset that provides information about the availaabillity, utilization and demand for EV charging infrastructure. This helps in a deeper understanding for the Local EV Market and thus helps researchers, analysts and businesses for sustainable transportation practices. This dataset contains the information on how much Energy is consumed in charging, how much GHG(Green House Gases) are saved by avoiding other fuel based vehicles. This helps to decide whether it is a better eco-friendly alternative or not.The dataset also includes the type of charging port, plugs, energy consumptions which enables to analyze the charging infrastructure performance. <br/>
* The dataset is of dimensions $259415\times33$. There are $259415$ instances of data and there are $33$ columns in each instance.<br/>
A summary of all the columns present in the dataset:
1. Station Name : Name of the EV Charging Station <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 47
2. MAC Address : MAC Address associated with Electric Charger <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 83
3. Org Name : City Name of charging station <br/> **Attribute Type**: Nomnial $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 1
4. Start Date : Start Data and  time stamp of charging <br/>**Attribute Type**: Interval scaled $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 244798
5. Start Time zone: Time zone where charging is being performed <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unqiue value counnt**:3
6. End Date : End Date and time stamp of charging <br /> **Attribute Type**: Interval scaled $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 244159
7. End Time zone: Time zone where charging is being ended <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 3
8. Transaction Date (Pacific Time): Transaction Date and Time <br/> **Attribute Type**: Interval scaled $\hspace{3cm}$ **Null count**: 209 <br/> **Unique value count**: 240905
9. Total Duration : Total Duration at the charging station <br/> **Attribute Type**: Interval scaled $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 31025
10. Charging Time : Time actually used for charging (can be less than total time) <br/> **Attribute Type**: Interval scaled $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 22473
11. Energy: Energy(in kwh) consumed for charging<br/> **Attribute Type**: Numerical $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 118061
12. GHG savings: Amount of Green House Gases(in KG) saved by using electricity instead of other fuels<br/> **Attribute Type**: Numerical $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 15535
13. Gasoline savings: Equivalent amount of Gasoline(in gallons) needed and saved <br/> **Attribute Type**: Numerical $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 6333
14. Port Type: Type of port used for charging(Level 1 or Level 2 port)<br/> **Attribute Type**: Binary $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 2
15. Port Number: Port Number used for charging <br/> **Attribute Type**: Binary $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 2
16. Plug Type: Type of plug used for charging($J1772$ or $NEMA 5-20R$)<br/> **Attribute Type**: Binary $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 2
17. EVSE ID: Electric vehicle Supply Equipment ID is a unqiue id for each charging point<br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 78948 <br/> **Unique value count**: 51
18. Address 1: Address of charging station <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 20
19. City: City where charging station is located <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 1
20. State/Province: Stat/Province where charging station is located<br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 1
21. Postal Code: Postal code of charging station location<br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 3
22. Country: Country of charging station<br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 1
23. Latitude: Latitude of charging station<br/> **Attribute Type**: Numerical $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 62
24. Longitude: Longitude of cahrging station<br/> **Attribute Type**: Numerical $\hspace{3cm}$ **Null count**: 0 <br /> **Unique value count**:64
25. Currency: type of currency used for transaction <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 1788 <br/> **Unique value count**: 4
26. Fee: Free amount for transaction<br/> **Attribute Type**: Numerical $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 1817
27. Ended by: How charging is ended  <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 248 <br/> **Unique value count**: 16
28. Plug In Event Id: unique ID for plugin event<br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 0 <br/> **Unique value count**: 36838
29. Driver Postal Code: Postal Code of location of driver <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 8402 <br/> **Unique value count**: 985
30. User Id: Id of user<br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 7677 <br/> **Unique value count**: 21441
31. County: The county(terrestrial division) to which chargin station belongs to <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 84665 <br/> **Unique value count**: 2
32. System S/N: System Serial Number <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 78948 <br/> **Unique value count**: 61
33. Model Number: Model Number of Charging Equipment <br/> **Attribute Type**: Nominal $\hspace{3cm}$ **Null count**: 78948 <br/> **Unique value count**: 10


## **Data Visualizations and insights through EDA**

Box plots for some of numerical columns: 
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/baa77f70-e50c-491d-822c-53b3efecd713) <br/>
The box plots show that the columns Energy, GHG Savings, Gasoline savings and Fee are all right(positive)-skewed datasets

Plots of GHG Savings vs Energy and Gasoline Savings vs Energy: 
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/b005b386-5ce1-4d23-ac79-7051901c3756) <br/>
The above graphs suggest that there is a strong correlation of Energy and GHG Savings 
<br/>
<br/>
Plot of Energy VS Fee:
<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/338dae55-9b5a-444c-b9ee-f8bfb3171a27)

Heat Map plot for correlation:<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/e361c6dd-e64d-4501-8d58-f76c37b44b98) <br/>
The above plot shows a perfect correlation among Energy, GHG Savings and Gasoline Savings.
Plot of Number of charging sessions recorded in each station: <br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/796a42e7-df88-49ad-a8a6-fda03e8ae5dc)
The maximum number of charging sessions are recorded in the station 'PALO ALTO CA / HAMILTON #2'

Pie chart of percentage distributions for port Types and plug Types:<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/aceec8f1-88a1-4151-8a2b-439cd34f0bc8) <br/>
Most of charging sessiosn use Level 2 Port Type and $J1772$ Plug Type.

Distribution of different types of currency usage in Transactions:<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/936ba2c6-a0b8-4f3d-91a7-db37e715c50a) <br/>
Due to larger difference of $USD$ and other currencies, the above plot is plotted using logarithmic scale!!!. 

Distribution of charging sessions in two different counties(terrestrial divisions):<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/00831e04-de3f-465a-8bec-de10bd7bef72) <br/>
Out of the two counties, majority of the charging sessions were recorded in Santa Clara County!!.

Histogram plot of charging time:<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/b2dcab1e-9bb6-4508-b1b1-e4024d63f981) <br/> 
From the above plot, most charging sessions take around 50minutes to 150 minutes for charging.

#### Summary of EDA Findings: 
1. The columns Energy consumption, GHG Savings and Gasoline savings are highly correlated with each other and thus 2 out of these 3 columns are redundant.
2. The maximum number of charging sessions are recorded in the station 'PALO ALTO CA / HAMILTON #2'
3. Most of charging sessions(Around $98%$) use Level 2 Port Type and Plug Type.
4. The columns Energy, GHG Savings, Gasoline savings, and Fee all have positively skewed distribution.
5. Most of the transactions recorded use $USD$ as currency
6. Out of the two counties, majority of the charging sessions were recorded in Santa Clara County!!.
7. Most charging sessions take around 50minutes to 150 minutes for charging.
8. There are no such interesting relations with latitude and longitude of charging station locations!!
9. Columns like City, State/Province, Country, Org name have only a single value for all the instances and thus not so useful in any analsysis. Thus they can be ignored.
10. Latitude and Longitude columns can be ignored as the information related to location can be captured from Staion Name itself.


## <center>Regression Problems<center>
The following regression problems can be solved using the given dataset:
1. **GHG Savings Prediction**: To predict the amount of Green House Gases(GHG) savings(in KG) of an electric vehicle charging session based on the charging session factors like Station Name,charging time, Total Duration, port Type, plug Type, Model Number, etc.
2. **Waiting time Prediction**: To predict the expected amount of waiting time(Total Duration - charging time) that a user has to spend at an EV Charging Station based on the charging session factors like Total Duration, Energy Consumption, port Type, plug Type, Model Number, Station Name and so on. This is same as predicting the expected charging time.
3. **Fee Prediction**: To predict the amount of fee charged for a session using the charging session factors like Energy, Charging Time, Station Name, Plug Type and Port Type and so on.
4. **Energy Prediction**: To predict the amount of Energy Consumed in a charging session based on charging time, total time, port type, plug type, charging station and so on.

Out of these above regression problems, predicting the amount of GHG savings seems most interesting as it helps in understanding the impact of EV Usage on Green House Gas Emissions and to compare the Electric vehicle emission with other fuel/petroleum based systems in terms related to pollution,etc. Furthermore, This problem involves removing correlated information about Energy and Gasoline saving and to do prediction based on other factors which don't have any direct correlation with GHG savings!!

## <center>End-to-End ML Pipeline <center>
The following are the steps taken in building an end-to-end ML pipeline for the problem of GHG Savings prediction:<br/>
#### Data preprocessing: <br/>
1. Removing columns that are not useful for prediction
2.  Replacing null values with mode for nominal attributes
3.  Converting Total Duration and Charging Time from $hh:mm:ss$ format to total number of seconds
4. Encoding nominal attributes using LabelEncoder()
The remaining data dimensions after data preprocessing is $(259415, 10)$. Now the data is ready for training.
#### Regression Model building
1. Train and test splitting: 80% of the data is used for training and 20% of the data is used for testing.
2. Data Normalization: Normalizing train and test data seperately using RobustScaler so that no data from test set will be leaked in training phase.
3. Model creation: The following models are used for training <br/> a. Lasso Regression<br/>b.Ridge Regression <br/> c. ElasticNet <br/> d. Stochastic Gradient Descent
4. Grid search for Hyperparameter tuning
5. Metrics used for optimization : Mean Squared Error(MSE), Mean Absolute Error(MAE) and Root Mean Squared Error(RMSE)
## Results: 
The following table shows the summary of training for each model.
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/be69216f-e1bd-4d01-8392-fca31bc7d72c)
Ridge Regression model has the best performance over the training data.
#### Evaluation
The performances of each model(with best hyperparameters) on test set are :<br/>
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/2e070603-54aa-4c7e-bd1e-7e55a543e1a2) <br/>
