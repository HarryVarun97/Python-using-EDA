OutPuts:

df.shape
(11251, 15)
df.head()
![Screenshot (546)](https://github.com/user-attachments/assets/2513c588-cdd6-4756-b480-002544d0d720)
df.info()
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 11251 entries, 0 to 11250
Data columns (total 15 columns):
 #   Column            Non-Null Count  Dtype  
---  ------            --------------  -----  
 0   User_ID           11251 non-null  int64  
 1   Cust_name         11251 non-null  object 
 2   Product_ID        11251 non-null  object 
 3   Gender            11251 non-null  object 
 4   Age Group         11251 non-null  object 
 5   Age               11251 non-null  int64  
 6   Marital_Status    11251 non-null  int64  
 7   State             11251 non-null  object 
 8   Zone              11251 non-null  object 
 9   Occupation        11251 non-null  object 
 10  Product_Category  11251 non-null  object 
 11  Orders            11251 non-null  int64  
 12  Amount            11239 non-null  float64
 13  Status            0 non-null      float64
 14  unnamed1          0 non-null      float64
dtypes: float64(3), int64(4), object(8)
memory usage: 1.3+ MB
pd.isnull(df).sum()
User_ID              0
Cust_name            0
Product_ID           0
Gender               0
Age Group            0
Age                  0
Marital_Status       0
State                0
Zone                 0
Occupation           0
Product_Category     0
Orders               0
Amount              12
dtype: int64
df['Amount'].dtypes
dtype('float64')
df['Amount'].astype(int)
0        23952
1        23934
2        23924
3        23912
4        23877
         ...  
11246      370
11247      367
11248      213
11249      206
11250      188
Name: Amount, Length: 11239, dtype: int32
df.columns
Index(['User_ID', 'Cust_name', 'Product_ID', 'Gender', 'Age Group', 'Age',
       'Marital_Status', 'State', 'Zone', 'Occupation', 'Product_Category',
       'Orders', 'Amount'],
      dtype='object')
df.rename(columns ={'Marital_Status':'Shaadi'})
![Screenshot (547)](https://github.com/user-attachments/assets/344006f2-c11f-4b16-bc34-e765a0b35bad)
df.describe()
![Screenshot (548)](https://github.com/user-attachments/assets/989730a3-92f4-4032-9601-88d5e3398930)
df[['Age','Orders','Amount']].describe()
![Screenshot (549)](https://github.com/user-attachments/assets/ca376837-aa6e-47ac-88a3-b3d710efefe0)

# Plotting a bar chart for Gender and it's count
![image](https://github.com/user-attachments/assets/190e1d36-21de-43ac-9647-a38d38d6b730)
# Plotting a bar chart for gender vs total amount
![image](https://github.com/user-attachments/assets/dc65e20f-276d-4435-b610-1482207c2371)
From above graphs we can see that most of the buyers are females and even the puchasing power of females are greater than  men
Age
![image](https://github.com/user-attachments/assets/36e786d6-b9b2-4cc0-b72c-9f917ea039e8)
# Total Amount vs Age Group
![image](https://github.com/user-attachments/assets/5d64852e-e578-44f4-bcc1-dbd031fdb564)
From above graphs we can see that most of the buyers are age group between 26-35yrs female
State
# total number of orders from top 10 states
![image](https://github.com/user-attachments/assets/d8a6a8e0-1a9d-4c44-8938-50b8463bc71a)
# total amount/sales from top 10 states
![image](https://github.com/user-attachments/assets/75589a64-0a27-4f57-a9d2-489055df6c4c)
From above graphs we can see that most of the  orders and total sales/amount are from Uttar  Pradesh, Maharashtra and Karnataka respectively
Marital Status
![image](https://github.com/user-attachments/assets/906ac390-41ca-41fd-a52f-182262969946)
![image](https://github.com/user-attachments/assets/c30543eb-e768-4166-bffe-e679aa423856)
From above graphs  we can see that  most  of  the buyers are married(women) and they have high purchasing power
Occupation
![image](https://github.com/user-attachments/assets/665cbc4d-e063-4959-9459-017bc90c515f)
![image](https://github.com/user-attachments/assets/1f97f16f-5499-4df2-a107-0b481307a57b)
From above graphs we can see that most of the buyers are working in IT, Healthcare and Aviation sector
Product Category
![image](https://github.com/user-attachments/assets/d7056af1-b97e-4f82-ab06-ab91f396a667)
![image](https://github.com/user-attachments/assets/16a4ecf9-16e3-4ffe-8406-ae4dd4ab00ea)
From above  graphs we can see that most of the sold products are from Food, Clothing and  Electronics category
![image](https://github.com/user-attachments/assets/6bc64d96-a542-4974-a857-34fe031bf176)
# top 10 most sold products (same thing as above)
![image](https://github.com/user-attachments/assets/caaa2964-3342-4f78-8471-c054758177eb)


#Conclusion:#
Married women age group 26-35 yrs from UP, Maharastra and Karnataka working in IT, Healthcare and Aviation are more likely to buy products from Food, Clothing and Electronics category


Thank you!











