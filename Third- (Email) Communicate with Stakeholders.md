Subject: Insights on Dove's Performance and Request for Additional Information
To: Adam
C.C.: Fetch Product Team(Dove), Data Analytics Team

Hi Adam,

I hope this message finds you well.

As we prepare to renew the contract with Dove next January, I would like to share some insights from my recent investigation into Dove's sales performance. I noted outstanding results in July regarding total sales and average daily sales. I hope these findings will assist your team in the negotiation process and help foster a strong collaborative relationship with Dove.

First, I want to highlight some data quality issues present in the dataset. While we will work to address these problems, I wanted to share them with you in advance to help you better understand the analysis and the potential risks involved.

* Key Data Quality Issues
During my analysis, I identified several important data quality issues that we need to address:
1.	Missing Values: There are several missing values in important variables across our datasets, especially in categorical data like users' STATE, GENDER, and LANGUAGE. We need to find the best way to handle these missing values, as simply filling them in could lead to misleading results.
2.	Duplicate Values: I found duplicate entries in both the 'Transaction' and 'Product' datasets. To ensure our analysis is accurate and to prevent any errors, I have removed these duplicate rows.
3.	Data Types: Some variables in the "Transaction" dataset, such as 'BARCODE,' 'FINAL_SALE,' and 'FINAL_QUANTITY,' have incorrect data types. This can lead to incorrect analysis and may also use up unnecessary memory.
4.	Data Entry Issues: I noticed some data entry problems in the 'Transaction' dataset. For example, 'FINAL_QUANTITY' should be numeric, but it includes entries with the string 'zero.' Additionally, there are blank entries in 'FINAL_SALE,' which makes it unclear whether they represent zero, unknown values, or mistakes.
5.	Data Completeness: Most user information in "TRANSACTION_TAKEHOME.csv" is missing from "USER_TAKEHOME.csv." If we can get more user data from the "Transaction" dataset, it would greatly improve our understanding of how users interact with Dove products, which is crucial for marketing strategies and user segmentation.
Interesting Trend
The performance of Dove in July was notably strong, particularly for Body Wash and Bar Soap, which have consistently ranked as the top products in their categories from June to September. However, I noticed that Women’s Deodorant dropped to second place in July, with the "Secret" brand surpassing Dove. This trend prompts further investigation into potential factors contributing to this change.
Request for Action
To dive deeper into these trends and improve our insights, I would appreciate your assistance with the following:
1.	Fetch’s Monthly Offers: Could you provide details on the offers available each month? Understanding these offers may help explain the observed differences in sales.
2.	Extended Transaction Data: Access to longer-term transaction data would allow us to analyze potential seasonality effects.
3.	Complete User Information: It would be helpful to obtain complete user profiles that match the transaction data. Additionally, knowing whether users saved Dove offers to their “like list” could clarify if these purchases were intentional or coincidental.
4.	“Secret” Brand Offers: Finally, understanding the offers provided for the “Secret” brand from June to September may help us explain why Dove’s Women’s Deodorant saw a decline in ranking.
Thank you for your attention to these matters. Your insights and any additional information you can provide will be invaluable in resolving these issues and further understanding the dynamics of Dove’s performance.
Best regards,
