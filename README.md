# Health Insurance Cross Sell Prediction

Lets assume that our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.
Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

Now, in order to predict, whether the customer would be interested in Vehicle insurance, we have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.

In this notebbok I'm analyzing different machine learning architectures, doing feature engineering etc with the goal to maximize ROC AUC score (which usually being used for similar tasks). However in this case the classes are really unblanced (Positive respones is around 10% only), so while AUC above 85% is being achieved with baseline models it does  not quite reflect the precision of the prediction - F1 score is less than 8%. 
Only after applying over-sampling can we improve precision to about 45%, while AUC reaches almost 88%.
It is understandable that we can reach slightly better results with parameters tuning, however I'm planning on doing it in the last stages of the development. First priority is to improve the predction through feature engineering.
