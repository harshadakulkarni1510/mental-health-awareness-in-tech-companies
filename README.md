# mental-health-data-analysis-in-tech-companies
Data Analysis using Python and machine learning techniques in Jupyter notebook to explore the dataset and uncover interesting trends & insights regarding the awareness of employees' mental health in tech companies 


## Background

Tech companies have been very popular employers in the past decade not just due to the boom in technological innovations but also because of attractive compensation and benefits packages. These employers have been known to offer various health benefit facilities, awareness programs and community groups to make sure their employees' physical health is taken care of. But when we talk about health, its not always just physical ailments that affect a person's personal or professional life. A lot of times, dealing with difficult events and enduring high level of stress causes mental health issues that go unnoticed or untreated. Creating awareness around mental health illnesses within employees and encouraging supportive conversations around such issues can help create a much positive impact on people's personal life resulting in betterment of their professional performance as well.

## Tools and techniques used

1. Jupyter Notebook
2. Python for Data Analysis (Pandas, numpy, scikitlearn, matplotlib, seaborn)
3. Machine learning techniques like linear & logistic regression, decision tress and k means clustering


## Datasets 

● 1 CSV file - Mental Health in Tech companies

● Datasource- Kaggle (3000 rows, 25 features)

● Major features - family history, treatment, age, no_of_employees, coworker, Supervisor


## Data Cleaning

1. Created age range -  pd.cut
2. Applied a function to convert categorical values to numerical values
3. Dealt with null values - df.fillna
4. Adjusted number of employees column using df.column.replace


## General trends in the dataset 

1. Distribution of age of people who took the survey - sns.distplot                
Most people who took the survey were between ages 25 to 45
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/26b47c52-ae2a-4e52-92fc-3e306da28cdb)


2. Distribution of percentage of Gender of people taking survey - groupby, sns.factorplot            
The gender ratio for people who took the survey was Male > Female > Others
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/57ad43d4-2dff-4d33-af77-11a790469e7d)


3. Country-wise percentage of distribution of mental illness           
The trend in amount of employees battling mental illness based on countries was Australia > US > UK > Netherlands > Ireland
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/d138f22f-fca9-41c1-bf1c-8f6882722ca0)


4. State-wise percentage of distribution of mental illness in U.S             
The trend in amount of employees battling mental illness in the US based on states was IL > CA > TX > OR > PA
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/413d1368-3781-4262-b6d1-6e5efd04b4a6)


5.Percentage of people for whom mental health issues interfere with work     
Amount of employees who found their mental health issues affecting their worklife based on gender was Others > Female > Male
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/a0a65a75-b72a-42e8-96f8-77ce775b3fde)


6. Linear Relation of Family History of mental illness Vs. treatment   
Employees with family history of mental health illnesses were seen to be more prone to developing mental health issues
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/7647d576-21ce-43b5-ab41-66f925d86be5)



## Insights

1. Size of the company    
People working in smaller companies are more willing to talk to other people about mental health issues vs. people working in larger organizations, despite of larger organizations spending more on mental health awareness and benefits. Even though 'bigger company = more benefits and encouragement to talk about issues' , data shows that  'smaller company = more people willing to talk about mental issues'
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/a4f445e9-bbae-487f-bb61-51a1e3b61788)
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/4cf5627c-3e50-4e9a-b358-0c7437805315)
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/92526ff2-82be-42fb-8197-8c99394d68d3)


        
2. Age of employees   
Although graphical representation and statistics might suggest that Age has a linear relation with Treatment, after using Logistic regression to find out class weights we can see out that Treatment depends much more on factors like family history, work interference etc. Even though 'Higher occurrence of mental issues = linear correlation to Age', data shows that class weight of Age lower than other factors like family history, gender, etc

![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/5047845a-785d-4e78-8441-69073be7025b)
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/ed2a0816-4b0f-4bd0-9ae0-1c1bf96b7db5)


                  
4. Aversion to talking about mental health    
Although people believe that their respective employers give equal importance to both mental and physical wellness, they are still less willing to talk about the topic when asked about it in a formal setting. After evaluating employees' mental vs physical health interviews using k means clustering, the data shows that people are less inclined to talk about mental health issues even after knowing that their company gives equal importance to both physical & mental health
![image](https://github.com/harshadakulkarni1510/mental-health-in-tech-companies/assets/158090021/3332396c-feb7-43cb-b851-f63be2f15008)







