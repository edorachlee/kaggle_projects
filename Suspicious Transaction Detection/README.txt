Kaggle API call: kaggle kernels output changhilee/suspicious-transaction-detection -p /path/to/dest

File descriptions:
train.csv - the training set
test.csv - the test set
sampleSubmission.csv - a sample submission file in the correct format

Data fields:
Target - In the training set, it implies whether the transaction is a fraud(Target = 1) or not(Target = 0). In your submission, it should be the estimated probability of a transaction is a fraud.
Timestamp - A masked time records when the transaction is made. Please note that this is not the real time, just indicating the relative time line.
Amount - How much money is involved in a transaction.
Goods - What kind of product or service is involved in a transaction.
T_0 - T_14 - Time related features, such as the frequency of customer using the same card.
C_0 - C_28 - Card related features, such as the type of the card.
V_0 - V_338 - Some evaluations the payment service company have on a transaction.
O_0 - O_39 - Card owner's information, such as the living address zipcode.
A_0 - A_1 - Address related features, such as where the transaction is made.
E_0 - E_1 - Email related features, E0 - to which email domain should the receipt be sent, E1 - card owner's email address domain.
M_0 - M_1 - On which device the transaction is made. M_0: mobile, desktop etc. M_1: additional info about the device, if any.

Categorical Data (inclusive): 
Goods
A_0, A_1
E_0, E_1
M_0, M_1
C_0 - C_8
C_23 - C_28
O_2, O_4, O_6-O_8
O_10 - O_17, O_19
O_21, O_23 - O_28
O_30 - O_32, O_35, O_36, O_39