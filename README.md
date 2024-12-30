<div align="center">
  <h1><b>Telecom Churn Prediction</b></h1>
</div>


![image](https://github.com/user-attachments/assets/fcbae31f-238e-47c4-9284-1164d6df8dee)

## What is Customer Churn?
Customer churn is defined as when customers or subscribers discontinue doing business with a firm or service.

Customers in the telecom industry can choose from a variety of service providers and actively switch from one to the next. The telecommunications business has an annual churn rate of 15-25 percent in this highly competitive market.

Individualized customer retention is tough because most firms have a large number of customers and can't afford to devote much time to each of them. The costs would be too great, outweighing the additional revenue. However, if a corporation could forecast which customers are likely to leave ahead of time, it could focus customer retention efforts only on these "high risk" clients. The ultimate goal is to expand its coverage area and retrieve more customers loyalty. The core to succeed in this market lies in the customer itself.

Customer churn is a critical metric because it is much less expensive to retain existing customers than it is to acquire new customers.

To detect early signs of potential churn, one must first develop a holistic view of the customers and their interactions across numerous channels.As a result, by addressing churn, these businesses may not only preserve their market position, but also grow and thrive. More customers they have in their network, the lower the cost of initiation and the larger the profit. As a result, the company's key focus for success is reducing client attrition and implementing effective retention strategy.
## Objectives:
- Finding the % of Churn Customers and customers that keep in with the active services.
- Analysing the data in terms of various features responsible for customer Churn
- Finding a most suited machine learning model for correct classification of Churn and non churn customers.

## Dataset:
[Telcom Customer Churn](https://github.com/Munnir-pasha/Telecom-Churn/blob/main/Data%2BDictionary-%2BTelecom%2BChurn%2BCase%2BStudy%20(2)%20(1).xlsx)


### The data set includes information about:
- Customers who left within the last month – the column is called Churn
- Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
- Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
- Demographic info about customers – gender, age range, and if they have partners and dependents
  
## Implementation:

Libraries: sklearn, Matplotlib, pandas, seaborn, and NumPy

## Few glimpses of EDA:
### 1. Churn distribution:
   ![image](https://github.com/user-attachments/assets/cf9a8ae8-276b-47a9-8509-49890afe36c2)
   26.6 % of customers switched to another firm.

### 2. Churn distribution with respect to gender:
![image](https://github.com/user-attachments/assets/3c7e82ea-61d6-4f38-bd57-3bf68f292f4c)

There is negligible difference in customer percentage/count who chnaged the service provider. Both genders behaved in similar fashion when it comes to migrating to another service provider/firm.`

### 3. Customer Contract distribution:
![image](https://github.com/user-attachments/assets/3fe041ec-7596-4148-9f43-ff150d61da01)

About 75% of customer with Month-to-Month Contract opted to move out as compared to 13% of customrs with One Year Contract and 3% with Two Year Contract
### 4. Payment Methods:
![image](https://github.com/user-attachments/assets/b609d099-0e76-4a46-9d02-1d4ae5e23346)

![image](https://github.com/user-attachments/assets/8bab01fe-c559-4d2f-b61b-6089a466f7f2)

Major customers who moved out were having Electronic Check as Payment Method. Customers who opted for Credit-Card automatic transfer or Bank Automatic Transfer and Mailed Check as Payment Method were less likely to move out.
### 5. Internet services:
Several customers choose the Fiber optic service and it's also evident that the customers who use Fiber optic have high churn rate, this might suggest a dissatisfaction with this type of internet service. Customers having DSL service are majority in number and have less churn rate compared to Fibre optic service.
![image](https://github.com/user-attachments/assets/8520b910-083c-4aff-91d7-c1d4a967b236)

### 6. Dependent distribution:
Customers without dependents are more likely to churn. Churn distribution w.r.t dependents

### 7. Online Security:
As shown in following graph, most customers churn due to lack of online security
![image](https://github.com/user-attachments/assets/7a5ecce8-aeae-49e6-8f00-f36071b689ce)

### 8. Senior Citizen:
Most of the senior citizens churn; the number of senior citizens are very less in over all customer base.
![image](https://github.com/user-attachments/assets/060430bf-b32a-4d45-8791-68d0df72daec)

### 9. Paperless Billing:
Customers with Paperless Billing are most likely to churn.
![image](https://github.com/user-attachments/assets/92499719-2efa-4351-b6a8-7a259198f1ed)

### 10. Tech support:
As shown in following chart, customers with no TechSupport are most likely to migrate to another service provider.
![image](https://github.com/user-attachments/assets/fd44f1d5-a2c5-4761-80dc-49eb8e433825)

### 11. Distribution w.r.t Charges and Tenure:
![image](https://github.com/user-attachments/assets/d30233e4-73de-42fd-a724-313ca73cd778)
![image](https://github.com/user-attachments/assets/58ea7b6d-6840-41b3-97c7-2e486e8eeb7f)
![image](https://github.com/user-attachments/assets/618e2a47-f666-49dc-8944-a266a9b99b19)

Customers with higher Monthly Charges are also more likely to churn.
New customers are more likely to churn.

## Machine Learning Model Evaluations and Predictions:
![image](https://github.com/user-attachments/assets/cb2dbb37-e79b-41da-a858-a04622aa0908)

### Results after K fold cross validation:
![image](https://github.com/user-attachments/assets/ac508ade-bfb1-47d6-befa-604800fcdb72)
![image](https://github.com/user-attachments/assets/742cf6de-377a-4f45-af8d-0c5084536f60)
![image](https://github.com/user-attachments/assets/2e0aa7ad-d0e6-4bf4-843e-fea39a833931)
![image](https://github.com/user-attachments/assets/20799d31-2ba3-4258-8496-bafaaa7be57e)
![image](https://github.com/user-attachments/assets/256f6065-3315-4ecf-ba7c-aa438a432633)
![image](https://github.com/user-attachments/assets/91590645-a698-41a9-8871-8d633fad243a)
![image](https://github.com/user-attachments/assets/4cc207de-d1d6-4e76-84c0-18e7ce4b1cac)
![image](https://github.com/user-attachments/assets/f9f2b1ee-2a8e-49eb-964a-b7ce31e34bda)
![image](https://github.com/user-attachments/assets/e9e68ebc-eee7-48a0-9a68-2b60aac23113)

### Final Model: Voting Classifier
  - We have selected Gradient boosting, Logistic Regression, and Adaboost for our Voting Classifier.
    ```python
    from sklearn.ensemble import VotingClassifier
    clf1 = GradientBoostingClassifier()
    clf2 = LogisticRegression()
    clf3 = AdaBoostClassifier()
    eclf1 = VotingClassifier(estimators=[('gbc', clf1), ('lr', clf2), ('abc', clf3)], voting='soft')
    eclf1.fit(X_train, y_train)
    predictions = eclf1.predict(X_test)
    print("Final Accuracy Score ")
    print(accuracy_score(y_test, predictions))
    ```

```python
Final_Score
{'LogisticRegression': [0.841331397558646, 0.010495252078550477],
    'KNeighborsClassifier': [0.7913242024807321, 0.008198993337848612],
    'GaussianNB': [0.8232386881685605, 0.00741678015498337],
    'DecisionTreeClassifier': [0.6470213137060805, 0.02196953973039052],
    'RandomForestClassifier': [0.8197874155380965, 0.011556155864106703],
    'AdaBoostClassifier': [0.8445838813774079, 0.01125665302188384],
    'GradientBoostingClassifier': [0.844630629931458, 0.010723107447558198],
    'VotingClassifier': [0.8468096379573085, 0.010887508320460332]}
```
 - Final confusion matrix we got:
    
    ![image](https://github.com/user-attachments/assets/8a374d08-7fa1-4e52-aa32-f74d1a0efe6d)

   
    From the confusion matrix we can see that: There are total 1383+166=1549 actual non-churn values and the algorithm predicts 1400 of them as non churn and 149 of them as churn. While there are 280+280=561         actual churn values and the algorithm predicts 280 of them as non churn values and 281 of them as churn values.
   

## Optimizations

We could use Hyperparamete Tuning or Feature enginnering methods to improve the accuracy further.

### Feedback
If you have any feedback, please reach out at Mohammadmunnir@outlook.com

### 🚀 About Me
Hi, I'm Munnir! 👋
I am an AI Enthusiast and Data science & ML practitioner

