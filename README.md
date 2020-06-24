# Pymaceuticals

The goal of this project was to calculate and display various performance metrics for four pharmaceutical cancer treatments (Capomulin, Infubinol, Ketapril, Placebo) on test mice over a 45 day treatment period. Since the baseline data was provided in CSV format, Python with Pandas, Numpy, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as calculate and display the desired outputs.

# Questions

For each treatment, what was the tumor volume change in the test mice over the length of the treatment period?
For each treatment, what was the metastatic site change in the test mice over the length of the treatment period?
For each treatment, what was the survival rate of the test mice over the length of the treatment period?
For each treatment, what was the percent change in tumor volume in the test mice over the length of the treatment period?

# Tasks

## Tumor Response to Treatment

Import the mouse data and clinical data CSV files as individual Pandas data frames.
Merge the individual data frames into a combined data frame based on the unique mouse identification numbers.
Split the combined data frame into groups by treatment and time index.
Calculate the average mean tumor volume for each treatment at each time index.
Calculate the tumor volume standard error for each treatment at each time index.
Create individual data frames for the average volume and standard error data.
Plot the average volume data versus time with error bars defined by the standard error data.
Metastatic Spread During Treatment
Split the combined data frame into groups by treatment and time index.
Calculate the average number of metastatic sites for each treatment at each time index.
Calculate the metastatic site standard error for each treatment at each time index.
Create individual data frames for the average metastatic site and standard error data.
Plot the average metastatic site data versus time with error bars defined by the standard error data.
Survival During Treatment
Split the combined data frame into groups by treatment and time index.
Calculate the number of surviving mice for each treatment at each time index.
Create a data frame for the survivng mice data.
Plot the surviving mice data versus time.
Tumor Change Over 45 Day Treatment
Calculate percent change in average tumor volume data over the full length of the treatment period.
Plot the percent change data for each treatment.

# Observations

Looking at the tumor volume change over time for each treatment, it is clear that Capomulin had the greatest positive effect on shrinking cancer cells. Total tumor volume in the mice receiving Capomulin dropped by just under 10 mm3 on average over the forty-five day test period. In contrast, total tumor volume in the mice receiving Infubinol, Placebo, or Ketapril increased by 20, 22.5, and 25 mm3 respectively throughout the study. This data, additionally supported by the tumor volume percent change data, clearly shows that Capomulin is the drug of choice for shrinking these cancerous tumor cells.

![image](https://user-images.githubusercontent.com/54809591/80607537-9eae9d00-8a03-11ea-85f8-8803319d2618.png)

Picking the most effective drug of the group is slightly more challenging when it comes to the data comparing metastatic sites versus time. All four of the treatments in question showed metastatic site increases, but two stood out in particular as being better. Capomulin did have the lowest increase at 1.5 sites, while Infubinol wasn't far behind at 2. They were followed by Ketapril and Placebo both around 3.25, which clearly weren't as effective. Therefore, none of the treatments were able to prevent metastatic site increases.

![image](https://user-images.githubusercontent.com/54809591/80607943-17adf480-8a04-11ea-99c5-8e5567e21a73.png)

Similar to the tumor volume change data, the mice survival rate data shows Capomulin had a clear advantage over the other three treatments. Over the length of the study, more mice treated with Capomulin survived and this effect was becoming evident even after the first ten days. At the end of the forty-five day period, over 80 percent of the mice on Capomulin survived compared to under 50 percent for Infubinol, Ketapril, and Placebo. Therefore, it was once again proven that Capomulin is the best choice for reducing the spread of these cancer cells and increasing the survival rate.

![image](https://user-images.githubusercontent.com/54809591/80608117-55ab1880-8a04-11ea-8f6e-3387242e0a11.png)

# Disclaimer

The baseline data used for this analysis was provided by a third party source and its accuracy in relation to actual pharmaceutical cancer treatment data is unknown.
