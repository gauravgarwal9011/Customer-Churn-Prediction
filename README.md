# <div align="center">Customer Churn Prediction</div>
![Intro](https://raw.githubusercontent.com/gauravgarwal9011/Customer-Churn-Prediction/refs/heads/main/Images/Customer-churn.webp)

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
 [Telco Customer Churn](https://www.kaggle.com/bhartiprasad17/customer-churn-prediction/data)

### The data set includes information about:

- Customers who left within the last month – the column is called Churn
- Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
- Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
- Demographic info about customers – gender, age range, and if they have partners and dependents
## Implementation:

**Libraries:** sklearn, Matplotlib, pandas, seaborn, and NumPy



## Few glimpses of EDA:
### 1. Churn distribution:
> ![Churn distribution](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Screenshot%202025-02-11%20131859.png)
> 26.6 % of customers switched to another firm.

### 2. Churn distribution with respect to gender:
> ![Churn distribution wrt Gender](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Screenshot%202025-02-11%20132251.png)


> There is negligible difference in customer percentage/count who chnaged the service provider. Both genders behaved in similar fashion when it comes to migrating to another service provider/firm.`

### 3. Customer Contract distribution:
> ![Customer contract distribution](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Screenshot%202025-02-11%20132439.png)
> About 75% of customer with Month-to-Month Contract opted to move out as compared to 13% of customrs with One Year Contract and 3% with Two Year Contract

### 4. Payment Methods:
>  ![Churn wrt payment methods](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Payment%20method.png)

> Major customers who moved out were having Electronic Check as Payment Method.
> Customers who opted for Credit-Card automatic transfer or Bank Automatic Transfer and Mailed Check as Payment Method were less likely to move out.

### 5. Internet services:

> Several customers choose the Fiber optic service and it's also evident that the customers who use Fiber optic have high churn rate, this might suggest a dissatisfaction with this type of internet service.
> Customers having DSL service are majority in number and have less churn rate compared to Fibre optic service.
![Churn distribution w.r.t Internet services and Gender](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Internet.png)

### 6. Dependent distribution:

> Customers without dependents are more likely to churn.
![Churn distribution w.r.t dependents](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Dependents.png)

### 7. Online Security:

> As shown in following graph, most customers churn due to lack of online security
![Churn distribution w.r.t online security](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Online%20security.png)

### 8. Senior Citizen:

> Most of the senior citizens churn; the number of senior citizens are very less in over all customer base.
![Churn distribution w.r.t Senior Citizen](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Senior%20citizen.png)


### 9. Paperless Billing:

> Customers with Paperless Billing are most likely to churn.
![Churn distribution w.r.t mode of billing](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Paperless%20billing.png)

### 10. Tech support:

> As shown in following chart, customers with no TechSupport are most likely to migrate to another service provider.
![Churn distribution w.r.t Tech support](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Tech%20support.png)

### 11. Distribution w.r.t Charges and Tenure:
> ![Monthly Charges](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Monthly%20charges.png)
> ![Total Charges](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Total%20charges.png)
> ![Tenure](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Tenure.png)

> Customers with higher Monthly Charges are also more likely to churn.<br>
> New customers are more likely to churn.

### 12.Confusion Matrix

#### <div align="center">Logistic Regression</div>
![Confusion Matrix](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Logistic%20Regression.png)

#### <div align="center">Decision Tree</div>
![Confusion Matrix](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Decision%20Tree.png)

#### <div align="center">Random Forest</div>
![Confusion Matrix](https://github.com/gauravgarwal9011/Customer-Churn-Prediction/blob/main/Images/Random%20Forest.png)

### 13.Final Model: Random Forest Classifier
From the Above models, we can say that the Random Forest Model performs much better than the other models. Customer churn economically decreases the company's funds and affects it's profitability.
