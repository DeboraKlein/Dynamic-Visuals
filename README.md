# Dynamic Visuals with Bookmarks & Toggle Buttons in Power BI & SWITCH + SELECTEDVALUE – Creating Dynamic Measures in Power BI

Dynamic Visuals with Bookmarks & Toggle Buttons Use bookmarks and toggle buttons to switch between visuals, keeping dashboards intuitive and interactive for seamless data exploration.

SWITCH + SELECTEDVALUE – Dynamic Measures Apply DAX logic to let users dynamically select metrics like Total Cost, Total Discount, and Quantity Bought, ensuring personalized insights.


 **Enhancing Data Exploration** 

Today, I learned a great way to offer users flexibility in data visualization:

-  **Using bookmarks** to toggle between a map and bar chart, giving users control over how they view their data.  
-  **Adding two buttons** to make the toggle seamless, almost like a simple on/off switch for visuals.

This approach keeps dashboards **clean, intuitive, and interactive**, making it easier to analyze trends **spatially or numerically**!
# Dynamic Visuals with Bookmarks & Toggle Buttons in Power BI

 **Enhancing Data Exploration** 

Today, I learned a great way to offer users flexibility in data visualization:

-  **Using bookmarks** to toggle between a map and bar chart, giving users control over how they view their data.  
-  **Adding two buttons** to make the toggle seamless, almost like a simple on/off switch for visuals.

This approach keeps dashboards **clean, intuitive, and interactive**, making it easier to analyze trends **spatially or numerically**!

 [**Dashboard Link**](https://app.powerbi.com/view?r=eyJrIjoiMmQ4MWM0NDYtZTVhOC00MjllLThlMjItODY2MGY0NzZhM2FiIiwidCI6IjY1OWNlMmI4LTA3MTQtNDE5OC04YzM4LWRjOWI2MGFhYmI1NyJ9)   
 
 ![**Image Link**](https://github.com/user-attachments/assets/921eef33-fc2b-445f-92e5-4f1fb9cf9e22)


---

# SWITCH + SELECTEDVALUE – Creating Dynamic Measures in Power BI

⚡ **Customizing Metrics with User Selection** ⚡

A powerful technique I explored today: using **SWITCH + SELECTEDVALUE** to allow users to dynamically change the metric they want to analyze!

With this approach, users can swap between:  

✔ **Total Cost**  
✔ **Total Discount**  
✔ **Quantity Bought**  

🔎 Here’s a snippet of the **DAX logic**:

DAX
Option = SWITCH(
    SELECTEDVALUE(KPIs[New Values]),
    "Total Cost", [Total Cost],
    "Qty Bought", [Qty Buy],
    "Total Discount", [Discount]
)

Title = SELECTEDVALUE(KPIs[New Values]) & " by Supplier"


🔗 [**Dashboard Link**](https://app.powerbi.com/view?r=eyJrIjoiMmQ4MWM0NDYtZTVhOC00MjllLThlMjItODY2MGY0NzZhM2FiIiwidCI6IjY1OWNlMmI4LTA3MTQtNDE5OC04YzM4LWRjOWI2MGFhYmI1NyJ9)  
🖼️ [**Image Link**](![Graph change - Graph Change   Analysis Exchange by Debora Klein - Power BI - Google Chrome 08_06_2025 19_38_02](https://github.com/user-attachments/assets/f2a303b8-72e2-47a6-a788-80892260ffb2)
)
