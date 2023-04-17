# Customer360
This is a project that uses PySpark to transform raw data into useful data on the topic of Customer 360.

The first step of the project is to load data from CSV files, parquet files.

Once the data has been loaded, PySpark will be used to clean and normalize the data. Data preprocessing steps will include removing empty values, handling outliers, and bringing the data into a consistent format.

Next, analyses will be performed to transform raw data into useful information about customers. For example, customer information from different sources will be aggregated to create a customer 360 profile, including used time, most watch, taste, and other relevant information.

Finally, evaluate user behavior including activeness, clinginess, ... based on those metrics. 

### Data Processing:
**1. Log content**
- Log content schema:

![1](https://user-images.githubusercontent.com/57434654/232549814-e7073497-6188-4998-8b60-ed77a1bc5347.png)

- Log content raw data:

![3](https://user-images.githubusercontent.com/57434654/232550150-ffefb3be-93aa-428d-9843-b081eb993d0e.png)

- Types of AppName:

![4](https://user-images.githubusercontent.com/57434654/232550715-b418ce68-221f-48e5-b54d-8c29ac5e95b9.png)

- After cleaning data:

![5](https://user-images.githubusercontent.com/57434654/232551872-d1d1914f-a079-42eb-90cb-c14a27ec2cfd.png)

![6](https://user-images.githubusercontent.com/57434654/232551889-7f959518-e93b-4e28-9f14-0792a97452fe.png)

- Calculate Most watch, Taste. Calculate Type of user based on *Interquartile range* and from these infer activeness and clinginess:

![7](https://user-images.githubusercontent.com/57434654/232553755-8a2536a2-cbf0-44f7-a2d4-dcb4a58270e6.png)


**2. Log search**
- Log search raw data:

![8](https://user-images.githubusercontent.com/57434654/232554026-5894dcb4-2919-401e-90d2-932a1260b1fc.png)

- After cleaning data:

![9](https://user-images.githubusercontent.com/57434654/232554179-320b3e8b-a3e4-40fa-85cc-e1d5eb1cdc57.png)

**3. Final result:**


![10](https://user-images.githubusercontent.com/57434654/232554337-dca30c81-824f-4de7-a5ea-82cde702aa25.png)

