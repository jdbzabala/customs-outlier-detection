![customs](https://github.com/user-attachments/assets/9363e0bb-b404-429a-9375-1d663857dbf9)

# SUMMARY
This report is concerned with investigating customs data for the month of Febraury 2024. Due to the recent irregularities found on shipments tagged as shoes, eg. misdeclaration, fake goods,
data entry errors, this report will focus on footwear shipments. The primary goal is to detect anomalies in declared quantities and weights of the shipment through outlier analysis.  
- Filtered the dataset to include only footwear (7,028 shipments)
- Performed Elliptic Envelope, Isolation Forest, OCSVM, GMM
- Chose Elliptic Envelope as the most appropriate method.
- Predicted 71 Outliers
- Outliers were shipments with suspicious weights or quantities.
- Outliers are recommended to be inspected for misdeclaration of quantity, content, or worse contraband.

# RESULTS
![OLOL](https://github.com/user-attachments/assets/9ed0085c-0652-4964-9eb2-71bb37769e70)
- Elliptic Envelope followed the expected linear relationship of quantity and net mass.
- Isolation Forest was only able to capture outliers on the right side of the plot.
- OCSVM and GMM performed similarly, with OCSVM being more refined.
- Not practical to use GMM in this case since distribution does not seem to be multimodal.
