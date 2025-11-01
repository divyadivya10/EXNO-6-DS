# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

     import pandas as pd
     import seaborn as sns
     import matplotlib.pyplot as plt
     df=pd.read_csv("titanic_dataset.csv")
     df.head()

<img width="1242" height="213" alt="image" src="https://github.com/user-attachments/assets/c56a9119-e3de-4a1e-8b97-8d3b3c3f9c4f" />

     x=[1,2,3,4,5]
     y=[3,6,2,7,1]
     sns.lineplot(x=x,y=y)
     plt.title('Line Plot')

<img width="791" height="604" alt="image" src="https://github.com/user-attachments/assets/f79a0dee-70fa-4f4a-ab5e-22246d613872" />
     

     x=[1,2,3,4,5] 
     y1=[3,5,2,6,1]
     y2=[1,6,4,3,8]
     y3=[5,2,7,1,4]
     sns.lineplot(x=x,y=y1)
     sns.lineplot(x=x,y=y2)
     sns.lineplot(x=x,y=y3)
     plt.title('Multi Line Plot')  

<img width="745" height="580" alt="image" src="https://github.com/user-attachments/assets/39a8207e-8534-4018-96e7-71bce904f3b7" />


     plt.figure(figsize=(8,5))
     sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
     plt.title("Fare Of Passenger By Embarked Town"

     
<img width="935" height="639" alt="image" src="https://github.com/user-attachments/assets/6ceffa4b-2a64-41da-a7f8-76ddfccb7f74" />

    sns.scatterplot(x="Age", y="Fare", data=df)
    plt.title('Scatterplot of Age vs Fare')
    plt.show()

<img width="793" height="578" alt="image" src="https://github.com/user-attachments/assets/489e8296-bb81-4d4c-9cfa-cf5f561500fa" />

    sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
    plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
    plt.show()

<img width="769" height="576" alt="image" src="https://github.com/user-attachments/assets/ed11a327-60cf-41e8-98e8-5e32bedab401" />


     sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)

<img width="772" height="573" alt="image" src="https://github.com/user-attachments/assets/56dff7d5-f8e0-4968-bc76-9cfa24fb220b" />

    sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
    plt.title("Age By Passenger Class")

<img width="911" height="604" alt="image" src="https://github.com/user-attachments/assets/f9411b37-65ff-4c4b-bd65-16979794f499" />

     sns.violinplot(x="Pclass", y="Fare", data=df)
     plt.title('Violin Plot of Fare by Passenger Class')
     plt.show()

<img width="838" height="596" alt="image" src="https://github.com/user-attachments/assets/41968c72-c071-4fb9-bd24-92e98a70c43b" />

    sns.kdeplot(data=df['Age'], shade=True)
    plt.title('Density Plot of Passenger Ages')
    plt.show()

<img width="837" height="561" alt="image" src="https://github.com/user-attachments/assets/8e1be838-a2d3-4814-a85a-f2af385b5f24" />

     numeric_df = df.select_dtypes(include=['float64', 'int64'])
     corr_matrix = numeric_df.corr()
     sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
     plt.title('Heatmap of Titanic Dataset')
     plt.show()

<img width="765" height="553" alt="image" src="https://github.com/user-attachments/assets/dfdeb404-f318-4ceb-84c8-099e28716f57" />

    
# Result:
 The code were executed successfully.
 

