# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE 
  
     import pandas as pd
     df=pd.read_csv("/content/Data_set .csv")
     df
     df.head(10)
     df.info()
     df.isnull()
     df.isnull().sum()
     df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
     df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
     df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
     df.head()
     df['rating']=df['rating'].fillna(df['rating'].mean())
     df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean
     df.head()
     df['watchers']=df['watchers'].fillna(df['watchers'].median())
     df.head()
     df.info()
     df.isnull().sum()

# output

![310214758-1bb2c4b4-4a28-4802-af7b-c43285bf1094 (1)](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/e4dd3206-39fc-43b4-83aa-5cc7e7f3fdee)
![310214758-1bb2c4b4-4a28-4802-af7b-c43285bf1094](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/e3bfb971-4f37-4232-9354-ddbb82eda8c9)
![310214758-1bb2c4b4-4a28-4802-af7b-c43285bf1094](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/2b5c794a-0f11-43a4-9529-1f8ce5cf3f2e)
![310215210-76eb0cdf-8b71-46f0-9752-534195ad76c7](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/b6cb3f0b-4e13-4dcc-9ae8-38d746f39cb8)
![310215267-ac7fcee7-e75f-4654-be44-f2487f38e139](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/5584adf2-5eeb-406f-8ee8-191f2736e22a)
![310215300-2043f1e7-fd6f-4e2e-993a-764df7eb74db](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/36a39d7d-fb1b-4697-9e9f-ec96dc3f2007)
![310215343-da1027d7-68bd-443c-aa9f-374c44fe020f](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/a7b68596-c6b3-456d-ab77-61fea5fafb50)
![310215343-da1027d7-68bd-443c-aa9f-374c44fe020f](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/8a976467-021b-4ffb-a79e-42cda7cee00d)
![310215343-da1027d7-68bd-443c-aa9f-374c44fe020f](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/0473d45f-e910-4324-aad6-7b878907df60)
![310215343-da1027d7-68bd-443c-aa9f-374c44fe020f](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/fc100e71-c851-4738-a6db-20b99952bdbb)
![310215549-04abc817-c20a-4805-9047-994d831f8a01](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/f68b6d74-5344-4ca8-be2f-3b17bce90121)
![310215589-a3a9fedb-5394-410b-baa7-c9e371bb79a9](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/12d4bad2-ffd2-431d-9499-bbc458278d36)
![310215628-faddd1c6-c755-460a-91a0-971c00970665](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/dfa6dfda-beaf-4526-ad2f-3e3ce8366478)
![310215662-7e979fee-2726-4769-85f3-4d5fc0b5c567](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/500bcfc5-be2d-4172-94a7-f04422a092fe)
![310215696-8bf4467f-40eb-4f38-839a-46b91e882827](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/7162f6ec-3f08-40f8-b819-ec27c54fe3db)
![310215751-ce7c7bb9-a558-43dd-9764-7d6ef5a7cde6](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/95ecfb40-c36b-4d77-a62d-46235ebf9a94)
![310215796-11c5dc33-028e-47fd-8444-b8139c35b0f1 (1)](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/e5dd5046-f5a7-46f8-8dca-f27bd0eb042c)
![310215796-11c5dc33-028e-47fd-8444-b8139c35b0f1](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/df743e36-66e3-436d-bb00-834828567729)
![310215858-3e2460b2-dd85-45e6-9946-844b2fecce78 (1)](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/438fb7af-7f26-4d14-bb23-ebc63f0a3b69)
![310215858-3e2460b2-dd85-45e6-9946-844b2fecce78](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/3ad59f36-b6d9-4a6f-9200-8f7220ba5183)

# 2)Outlier Detection and Removal

# AIM
To read a given dataset and remove outliers and save a new dataframe.

# ALGORITHM:
(1) Remove outliers using IQR

(2) After removing outliers in step 1, you get a new dataframe.

(3) use zscore of 3 to remove outliers. This is quite similar to IQR and you will get exact same result

(4) for the data set height_weight.csv find the following

(i) Using IQR detect weight outliers and print them

(ii) Using IQR, detect height outliers and print them

# PROGRAM
      import pandas as pd
      import numpy as np
      import seaborn as sns
      import pandas as pd
      from scipy import stats
      df = pd.read_csv("/content/heights.csv")
      sns.boxplot(data=df)
      sns.scatterplot(data=df)
      max =df['height'].quantile(0.90)
      min =df['height'].quantile(0.15)
      max
      min
      dq = df[((df['height']>=min)&(df['height']<=max))]
      dq
      low = min-1.5*iqr
      high = max+1.5*iqr
      dq = df[((df['height']>=min)&(df['height']<=max))]
      dq

# ZSCORE:
      import pandas as pd
      import numpy as np
      import seaborn as sns
      import pandas as pd
      from scipy import stats
      data = {'weight':[12,15,18,21,24,27,30,33,36,39,42,45,48,51,54,57,60,63,66,69,202,72,75,78,81,84,232,87,90,93,96,99,258]}
      df = pd.DataFrame(data)
      df
      sns.boxplot(data=df)
      z = np.abs(stats.zscore(df))
      print(df[z['weight']>3])
      val =[12,15,18,21,24,27,30,33,36,39,42,45,48,51,54,57,60,63,66,69,202,72,75,78,81,84,232,87,90,93,96,99,258]
      out=[]
      def d_o(val):
      ts=3
      m=np.mean(val)
      sd=np.std(val)    
      for i in val:
      z=(i-m)/sd
      if np.abs(z)>ts:
      out.append(i)
      return out
      op = d_o(val)
      op

# OUTPUT
![310218959-e23d7d25-399e-4d85-aa06-0d2845e7dbc2](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/d3414cc1-7d2e-4261-886a-f8e23854e7bf)
![Screenshot 2024-03-07 094529](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/c1d105e1-5e56-433d-b0aa-9c0a78dcea7f)
![Screenshot 2024-03-07 094507](https://github.com/Mothykrishnan100/ODD2023-Datascience-Ex01/assets/160512502/b4b7dada-45c3-463a-8380-44df29c1a6fc)
# RESULT
Thus, the given data is read, cleansed and the cleaned data is saved into the file and the given data is read,remove outliers and save a new dataframe was created and executed successfully.
