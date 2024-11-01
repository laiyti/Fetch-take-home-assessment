## Subject: Insights on Dove's Performance and Request for Additional Information

#### To: Adam

#### C.C.: Fetch Product Team (Dove), Data Analytics Team


Hi Adam,

I hope this message finds you well.

As we prepare to renew the contract with Dove next January, I would like to share some insights from my recent investigation into Dove's sales performance for our users. I noted outstanding results in July regarding total sales and average daily sales. I hope these findings will support your team in the negotiation process and help foster a strong collaborative relationship with Dove.

First, I want to highlight some data quality issues present in the dataset. While we will work with engineering team to address these problems, I wanted to share them with you in advance to help you better understand the analysis and the potential risks involved.

 > __Key data quality issues:__

During my analysis, I identified several important data quality issues that we need to address:

1.	__Missing values__:
Several important variables across our datasets contain missing values, including users' information (state, gender, language), transaction barcodes, and product details (categories, manufacturer, and brand). This poses a risk of losing valuable insights; for instance, over 5,000 transactions lack barcodes, preventing us from identifying the products purchased by users.

2.	__Duplicate values__:
There are duplicate entries in both the 'Transaction' and 'Product' datasets. This issue can lead to calculation errors; for example, if a receipt for three Dove body soaps is recorded twice with the same product, quantity, and sale, our sales performance calculations may be overstated. To prevent this, I have already removed all duplicate records from the 'Transaction' and 'Product' datasets in the analysis provided here.

3.	__Data types & Data enry__:
Some variables in the "Transaction" dataset, such as 'BARCODE,' 'FINAL_SALE,' and 'FINAL_QUANTITY,' have incorrect data types, which can lead to calculation errors. For instance, some records in 'FINAL_QUANTITY' show 'zero' instead of 0. Although we can infer that 'zero' means 0, the system cannot perform calculations because it treats it as text. Additionally, some records in 'FINAL_SALE' contain just a space (' '), making it unclear whether they represent 0, unknown values, or entry errors.
For this analysis, we first removed records where 'FINAL_QUANTITY' = 'zero' or 'FINAL_SALE' = ' '. Based on our past experience, these are likely data entry errors. Our team will double-check with the engineering team and update you if any changes occur.

4.	__Data completeness__: 
The User dataset contains 100,000 users, but only 130 users match the Transaction data. This limited overlap makes it challenging to analyze deeper insights between transactions, products, and users. For instance, it will be difficult to answer questions such as: "What types of users prefer Dove's body soap?" This includes understanding factors like location, gender, and age.

5.	__Data accuracy__: I discovered that in the 'Product' dataset, both Dove soap and Dove chocolate are listed under the brand name 'DOVE.' We will discuss this discrepancy with the engineering team, as failing to address it could lead to incorrectly attributing Dove chocolate sales to Dove soap. For this analysis, I selected products under the 'Health & Wellness' category to ensure we are analyzing the correct products and transactions.


  > __Interesting Trend:__

After reviewing the data quality issues, I would like to share some interesting trends regarding Dove's sales performance from June 12 to September 8, based on the provided Transaction data.

The sales performance in each month shows below. 

<img width="355" alt="Screenshot 2024-11-01 at 1 43 43 PM" src="https://github.com/user-attachments/assets/c6a4b34e-27ac-4978-a6d5-eade7d4f9a5b">

As you see, the performance of Dove in July was notably strong.

To identify the popular products, we calculated the number of receipts for each product by month:

We found __Body Wash__, __Bar Soap__, and __Women’s Deodorant__ are the top 3 popular products.
<img width="713" alt="Screenshot 2024-11-01 at 1 54 50 PM" src="https://github.com/user-attachments/assets/f8d1e04b-1b0c-41ad-9b05-48de08ebae20">

Upon reviewing sales for these products each month, we observed that Body Wash and Bar Soap consistently ranked as the top products in their categories from June to September. However, Women’s Deodorant dropped to second place in July, with the "Secret" brand surpassing Dove.

  * Body Wash:
<img width="661" alt="Screenshot 2024-11-01 at 2 00 04 PM" src="https://github.com/user-attachments/assets/33eb918c-6eda-4070-b6c0-aab489479e45">

  * Bar Soap:
<img width="652" alt="Screenshot 2024-11-01 at 2 00 52 PM" src="https://github.com/user-attachments/assets/d78987b0-a315-410a-a134-c8bad0b00f69">

  * Women’s Deodorant: 
<img width="790" alt="Screenshot 2024-11-01 at 2 01 10 PM" src="https://github.com/user-attachments/assets/bacabd18-a574-42ca-bf7f-5218e78c6ee9">


  > __Request for Action:__

To dive deeper into these trends and improve our insights, I would appreciate your assistance with the following:

1.	__Fetch’s monthly Dove-related offers__: Could you provide details on the Dove-related offers available each month? Understanding these offers may help explain the observed differences in sales.
2.	__More Transaction data__: Access to longer-term transaction data would enable us to analyze potential seasonality effects. For example, we can determine if July consistently shows higher sales each year.
3.	__Complete user information__: Obtaining complete user profiles that match the transaction data would be beneficial. This information will help us understand the relationship between transactions, products, and users more comprehensively. Additionally, if we can demonstrate that our users align with Dove’s target audience, it could strengthen our negotiation position and foster a better partnership. If possible, knowing whether users saved Dove offers to their “like list” could clarify if these purchases were intentional or coincidental.
4.	__“Secret” brand offers__: Understanding the offers provided for the “Secret” brand from June to September may help explain the decline in Dove’s Women’s Deodorant ranking. If Dove seeks to strengthen their sales in this category, we can provide advice and observations based on our findings.

Your insights and any additional information you can provide will be invaluable in resolving these issues and deepening our understanding of Dove’s performance dynamics. Once we have more information, I can create dashboards for your team to present to Dove.

If you have any questions or need further clarification, please feel free to reach out or schedule a meeting with me.

Thank you for your attention to these matters. I look forward to your reply.

Best regards,

Yi-Ting Lai
