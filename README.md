# Matplotlib_Challenge
In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.
The provided data imports were ran. The two sets of data (mouse_metadata and study_results) were merged into a single DataFrame.
The unique mice IDs in the data were found, and then checked for any mouse ID with duplicate time points. The duplicate data was removed, and then a new DataFrame was created where the duplicate data was removed. 
This cleaned DataFrame was used for the remaining analysis.
Created a DataFrame of summary statistics. 
The summary statistics included:
A row for each drug regimen. These regimen names are contained in the index column.
A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.
Two bar charts were generated. Both charts are identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.The first bar chart was created with the Pandas DataFrame.plot() method.The second bar chart was created with Matplotlib's pyplot methods.
Two pie charts were created. Both charts are identical and show the distribution of female versus male mice in the study. The first pie chart was created with the Pandas DataFrame.plot() method. The second pie chart was created with Matplotlib's pyplot methods.
The final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin was calculated. Then, the quartiles and IQR, were calculated. Potential outliers across all four treatment regimens were identified.
A grouped DataFrame that shows the last (greatest) time point for each mouse was created. It was then merged with the original cleaned DataFrame. A list was created that holds the treatment names as well as a second, empty list to hold the tumor volume data.A for loop was created to loop through each drug in the treatment list. This located the rows in the merged DataFrame that correspond to each treatment. The resulting final tumor volumes for each drug wewre appended to the empty list.
Outliers were determined by using the upper and lower bounds.
Using Matplotlib,a box plot was generated that shows the distribution of the final tumor volume for all the mice in each treatment group. Any potential outliers were highlighted in the plot.
A single mouse (U363) was selected that was treated with Capomulin. A line plot of tumor volume versus time point for that selected mouse.
A scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen was created. The correlation coefficient and linear regression model was used to relation between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen. The linear regression model was also plotted along with the data points.

References

Cottontail.(2018, March 18). "Python-Grouping by multiple columns to find duplicate rows in pandas." Stackoverflow. https://stackoverflow.com/questions/46640945/grouping-by-multiple-columns-to-find-duplicate-rows-pandas

McKinney, T. (2021, August 6). "Python-how to use Pandas filter with IQR." Stackoverflow. https://stackoverflow.com/questions/34782063/how-to-use-pandas-filter-with-iqr

Hunter, J., Dale, D., Firing, E., Droettboom, M., the Matplotlib development team. "Title positioning." matplotlib. https://matplotlib.org/3.5.0/gallery/text_labels_and_annotations/titles_demo.html

Chakaraborty, S.(2020, December 11)."Line plot styles in Matplotlib." GeeksforGeeks. https://www.geeksforgeeks.org/line-plot-styles-in-matplotlib/

Dawda, S. (2018, January 21). "Pyton-how to add regression line and regression line equation on graph." Stackoverflow. https://stackoverflow.com/questions/48370562/how-to-add-regression-line-and-regression-line-equation-on-graph

Naveen, (NNK). (2023, January 28). "Pandas groupby() and sum() With Examples." Spark By {Examples}. https://sparkbyexamples.com/pandas/pandas-groupby-sum-examples/

DeMan, B.(2015, September 1). "How do I use matplotlib autopct?." Stackoverflow. https://stackoverflow.com/questions/6170246/how-do-i-use-matplotlib-autopct

Shivam_k, (2018, September 18). "Python | Pandas.pivot()." GeeksforGeeks. https://www.geeksforgeeks.org/python-pandas-pivot/
