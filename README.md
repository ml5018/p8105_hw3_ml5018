# p8105_hw3_ml5018

This is a README document for homework 3 of p8105, created by Luan Mengxiao.

Here list some basic requirements of this homework.

## Problem 0

This “problem” focuses on structure of your submission, especially the use git and GitHub for reproducibility, R Projects to organize your work, R Markdown to write reproducible reports, relative paths to load data from local files, and reasonable naming structures for your files.

To that end:

* create a public GitHub repo + local R Project; we suggest naming this repo / directory p8105_hw3_YOURUNI
* create a single .Rmd file named p8105_hw3_YOURUNI.Rmd that renders to github_document
* create a subdirectory to store any local data files, and use relative paths to access these data files
* submit a link to your repo via Courseworks

## Problem 1

This problem uses the Instacart data. DO NOT include this dataset in your local data directory; instead, load the data from the `p8105.datasets`.

The goal is to do some exploration of this dataset. To that end, write a short description of the dataset, noting the size and structure of the data, describing some key variables, and giving illstrative examples of observations. Then, do or answer the following (commenting on the results of each):

* How many aisles are there, and which aisles are the most items ordered from?
* Make a plot that shows the number of items ordered in each aisle, limiting this to aisles with more than 10000 items ordered. Arrange aisles sensibly, and organize your plot so others can read it.
* Make a table showing the three most popular items in each of the aisles “baking ingredients”, “dog food care”, and “packaged vegetables fruits”. Include the number of times each item is ordered in your table.
* Make a table showing the mean hour of the day at which Pink Lady Apples and Coffee Ice Cream are ordered on each day of the week; format this table for human readers (i.e. produce a 2 x 7 table).

## Problem 2

This problem uses the BRFSS data. DO NOT include this dataset in your local data directory; instead, load the data from the p8105.datasets package.

First, do some data cleaning:

* format the data to use appropriate variable names;
* focus on the “Overall Health” topic
* include only responses from “Excellent” to “Poor”
* organize responses as a factor taking levels ordered from “Poor” to “Excellent”
* Using this dataset, do or answer the following (commenting on the results of each):

* In 2002, which states were observed at 7 or more locations? What about in 2010?
* Construct a dataset that is limited to Excellent responses, and contains, year, state, and a variable that averages the data_value across locations within a state. Make a “spaghetti” plot of this average value over time within a state (that is, make a plot showing a line for each state across years – the geom_line geometry and group aesthetic will help).
* Make a two-panel plot showing, for the years 2006, and 2010, distribution of data_value for responses (“Poor” to “Excellent”) among locations in NY State.

## Problem 3

Accelerometers have become an appealing alternative to self-report techniques for studying physical activity in observational studies and clinical trials, largely because of their relative objectivity. During observation periods, the devices can measure MIMS in a short period; one-minute intervals are common. Because accelerometers can be worn comfortably and unobtrusively, they produce around-the-clock observations.

This problem uses accelerometer data collected on 250 participants in the NHANES study. The participants’ demographic data can be downloaded here, and their accelerometer data can be downloaded here. Variables *MIMS are the MIMS values for each minute of a 24-hour day starting at midnight.

Load, tidy, merge, and otherwise organize the data sets. Your final dataset should include all originally observed variables; exclude participants less than 21 years of age, and those with missing demographic data; and encode data with reasonable variable classes (i.e. not numeric, and using factors with the ordering of tables and plots in mind).

Produce a reader-friendly table for the number of men and women in each education category, and create a visualization of the age distributions for men and women in each education category. Comment on these items.

Traditional analyses of accelerometer data focus on the total activity over the day. Using your tidied dataset, aggregate across minutes to create a total activity variable for each participant. Plot these total activities (y-axis) against age (x-axis); your plot should compare men to women and have separate panels for each education level. Include a trend line or a smooth to illustrate differences. Comment on your plot.

Accelerometer data allows the inspection activity over the course of the day. Make a three-panel plot that shows the 24-hour activity time courses for each education level and use color to indicate sex. Describe in words any patterns or conclusions you can make based on this graph; including smooth trends may help identify differences.
