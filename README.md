A Sunday Predictive Maintenance Project by Oliver Kele

In this workbook, I'll be working with a synthetic predictive maintenance dataset from Kaggle (https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification). This dataset was created by UC Irvine to allow machine learning students to work with realistic predictive maintenance data, which is usually difficult to obtain (https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset).

This dataset has already been used widely to build machine learning models (there are 132 notebooks for this data on Kaggle), so I'll be taking a slightly different approach:

**What maintenance rules & best practices can be learnt from the data and communicated to operators?**

Here's my assumptions that lead me to pursue this research question:
* In the field, it may not always be possible to get reliable sensor data
* Operators of these machines (who are responsible for maintenance) likely do not have a machine learning background that allows them to effectively intepret complex model's outputs
* Organisations may favour simple but reliable rules that can be recorded in operator manuals and workplace health & safety documentation

I'm thinking about this problem like a pre-shift inspection. I don't need a super complicated machine learning model to tell me to check oil levels before I start a piece of machinery. However, I would like to know that if it's really cold I need to check my oil twice a day, or in certain conditions machines are prone to specific failure-modes.

This approach introduces a unique challenge: **I'm not just minimising loss, I'm also maximising explanability**.
