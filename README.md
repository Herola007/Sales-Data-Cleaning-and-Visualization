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
-After importing the second part of the dataset back into Power Query, we utilized the Transpose button under the Transform ribbon. This action transposed the table, resulting in the output shown in the image above.

![img_four](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(4).png?raw=true)
- A new column named Segment was added to the transposed table to categorize the modes of shipment.

![img_three](https://github.com/Herola007/Raye-Stores-Sales-Data-Cleaning-and-Visualization/blob/main/Steps/2024-10-09%20(3).png?raw=true)
-Next, I proceeded to unpivot the table, excluding the first two columns that were already pivoted. The image above illustrates the resulting table after this transformation. After completing the modifications for the second part of the dataset, I then loaded the data back into Excel.



