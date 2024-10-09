## Raye-Stores-Sales-Data-Cleaning-and-Visualization
**This repository provides a step-by-step guide on how Raye Stores' sales data was cleaned using Power Query and visualized using Power BI.** 

![Data cleaning](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Database%20Illustrator.jpg?raw=true)

### Project Overview
As a junior data analyst, I had the opportunity to work with Raye Stores to clean and restructure a poorly organized dataset provided by their sales department. The project's objective was clear: to transform the messy data into a well-structured format that could be used for effective analysis and reporting.

Upon receiving the dataset from the sales team, I immediately began the cleaning process. Using Power Query, I followed a methodical approach to ensure the data was accurate, and consistent, while also establishing a fixed schema for future analysis.

This repository provides a step-by-step walkthrough of the entire data cleaning process, showcasing how Power Query was utilized to handle various data issues. The final cleaned dataset was then prepared for further analysis and visualization in Power BI to extract actionable insights.


### Data Cleaning/Transformation
The dataset provided by the sales team came in a CSV format, which I initially opened using Microsoft Excel. To perform the necessary transformations, I imported the entire dataset into Power Query Editor, where I could take full control of the cleaning and transformation process. Although the dataset initially appeared chaotic, once imported, it became much more manageable within Power Query.

This section will detail the step-by-step process of how the data was transformed and cleaned. Screenshots will be provided throughout to visually illustrate each step, along with explanations of what actions were performed and why. At the end of this write-up, I will also include a screenshot of the applied steps in Power Query, summarizing the entire transformation process.

![img_zero](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-08%20(0).png?raw=true)
- The image above shows the badly structured data after importing into Power Query

The first image illustrates how data can be transferred from Excel into Power Query. To simplify the analysis process, I returned to Excel and split the dataset into two parts. This division made it easier to manage and clean the data effectively.

![img_one](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09(1).png?raw=true)
- The highlighted section in the image above indicates the portion of the dataset that will be separated from the larger dataset for further processing. The highlighted section is going to get imported back into Power Query.

![img_two](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(2).png?raw=true)
 - After importing the second part of the dataset back into Power Query, we utilized the Transpose button under the Transform ribbon. This action transposed the table, resulting in the output shown in the image above.

![img_four](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(4).png?raw=true)
- A new column named Segment was added to the transposed table to categorize the modes of shipment.

![img_three](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(3).png?raw=true)
 - Next, I proceeded to unpivot the table, excluding the first two columns. The image above illustrates the resulting table after this transformation. After completing the transformation for the second part of the dataset, I then loaded the data back into Excel.

After transforming the highlighted portion of the data shown earlier, we can now return to the original dataset to continue with the cleaning process. This step is crucial to ensure that all inconsistencies and inaccuracies are addressed, allowing for a more reliable analysis.

![img_five](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(5).png?raw=true)
- The image above displays the original dataset that requires transformation before we can proceed.

![img_six](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(6).png?raw=true)
- This image displays the result of pivoting the original dataset, excluding the first column. The first 18 rows will be deleted as they are irrelevant to the analysis, especially since we already have their descriptions in the second dataset.

![img_seven](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(8).png?raw=true)
- This is the result of our original dataset after being transformed. Now, we have two datasets in our Excel workbook, but both still contain duplicate values. The next step is to remove these duplicates to ensure the data is fully clean.

![img_eight](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(88).png?raw=true)
-This is our first dataset, transformed using Power Query, with each column properly renamed to reflect the appropriate titles. The dataset is now fully cleaned.

![img_nine](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(9).png?raw=true)
-This is our second dataset, which has also been transformed using Power Query, with each column appropriately renamed.

To merge the two datasets, we will use a lookup function—either XLOOKUP or the INDEX-MATCH function—to find the appropriate values for each OrderID. For this project, we’ll be using INDEX-MATCH, so let’s dive right into it.

![img_ten](https://raw.githubusercontent.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/refs/heads/main/Steps/2024-10-09%20(1010).png)

![img_eleven](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(1111).png?raw=true)

The segment for each Orderid has been successfully retrieved using the formula above. Next, we will use the same approach to find the Ship Mode for each Orderid.

![img twelve](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(12).png?raw=true)

![img_thirteen](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(13).png?raw=true)

![img_fourteen](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(14).png?raw=true)

This is the final result of our cleaned and transformed datasets, which will also be uploaded to this repository as a CSV file. We can now proceed to analyze and visualize this dataset using Microsoft Power BI.

![Dashboard Screenshot](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Dashboard%20Screenshot.png?raw=true)



