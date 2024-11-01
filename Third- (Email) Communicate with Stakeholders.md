Subject: Insights on Dove's Performance and Request for Additional Information

To: Adam

C.C.: Fetch Product Team(Dove), Data Analytics Team

Hi Adam,

I hope this message finds you well.

As we prepare to renew the contract with Dove next January, I would like to share some insights from my recent investigation into Dove's sales performance for our users. I noted outstanding results in July regarding total sales and average daily sales. I hope these findings will assist your team in the negotiation process and help foster a strong collaborative relationship with Dove.

First, I want to highlight some data quality issues present in the dataset. While we will work with engineering team to address these problems, I wanted to share them with you in advance to help you better understand the analysis and the potential risks involved.

* __Key data quality issues:__

During my analysis, I identified several important data quality issues that we need to address:

1.	__Missing values__: There are several missing values in important variables across our datasets, such as users' information(state, gender, language), transactions' barcode, products' detail categories, manufature and brand. The potential risk for this issue is we might lose some important insights because we don't have the details. For example, there are over 5000 transactions without barcode, then we would not know which products the users bought, we might lose some important insight due to this issue.

2.	__Duplicate values__: There are duplicate entries in both the 'Transaction' and 'Product' datasets. This issue might cause some calculation error, for example, if there is one receipt buying 3 Dove's body soap, but the same receipt with the exactly same product, quantity and sale show twice, then when we calculate the sales performance, we might overestimate the sales due to this issues. To prevent this, the analysis I provided here has already removed all of the completely same records in 'Transactions' and 'Product' datasets.

3.	__Data types & Data enry__: Some variables in the "Transaction" dataset, such as 'BARCODE,' 'FINAL_SALE,' and 'FINAL_QUANTITY,' have incorrect data types, which might also cause calculation error. For example, there are some records in 'FINAL_QNANTITY' show 'zero' instead of 0. Even thoguh we can guess zero means 0, the computer will not be able to calculate this because it thinks number can not add with a word. Besides, there are some records containing just a space (' ') in 'FINAL_SALE,' which are problematic because it is unclear whether they represent 0, unknown values, or entry errors. For this analysis, we removed the records with 'FINAL_QUANTITY' = 'zero' or 'FINAL_SALE' = (' ') first, because based on our past experience it is highly possible that it's error while entering the data. Our team will double check with the engineering team, and let you know if there's any change.

5.	__Data completeness__: 
While in the User dataset provided have 100000 users, there are only 130 users matches the Transaction data. That means based on what we have now it will be hard to further analyze the deeper insights between transactios, products, and the user. For example, it will be hard to answer the question: Dove's body soap is most popular to what kind of users? (it can be live where, which gender, and the age.)

* __Interesting Trend:__
After you understand some backgroud data quality issue, I would like to share some interesting trend.

The performance of Dove in July was notably strong, particularly for Body Wash and Bar Soap, which have consistently ranked as the top products in their categories from June to September. However, I noticed that Women’s Deodorant dropped to second place in July, with the "Secret" brand surpassing Dove. This trend prompts further investigation into potential factors contributing to this change.


* __Request for Action:__
To dive deeper into these trends and improve our insights, I would appreciate your assistance with the following:

1.	__Fetch’s monthly Dove-related offers__: Could you provide details on the dove-related offers available each month? Understanding these offers may help explain the observed differences in sales.
2.	__More Transaction data__: Access to longer-term transaction data would allow us to analyze potential seasonality effects. For example, is it common to see July have higher sales every year or not.
3.	__Complete user information__: It would be helpful to obtain complete user profiles that match the transaction data. As mentioned above, it will help us to better understand the relationship between transactions, products and users. We can provide more detail pictures about users, which will also be what Dove care about. If we can prove our users matches their target users, it will be helpful for us to negotiate and build even stronger relationship. Additionally, if it's possible knowing whether users saved Dove offers to their “like list” could clarify if these purchases were intentional or coincidental.
4.	__“Secret” brand offers__: Finally, understanding the offers provided for the “Secret” brand from June to September may help us explain why Dove’s Women’s Deodorant saw a decline in ranking. If Dove would like to strengthen their sales in Women's Deodorant, then we can provide some advices and observations in advance.

Thank you for your attention to these matters. Your insights and any additional information you can provide will be invaluable in resolving these issues and further understanding the dynamics of Dove’s performance.
If you have any questions or need further explaination, please feel free to reach out or schedule a meeting with me.

Best regards,

Yi-Ting Lai
