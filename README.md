# python-api-challenge

I started the api challenge by creating a repo on github and cloned to my PC. Using gitbash I used the function mkdir to created the required directories/folders and nested them under the matplotlib-challenge main folder. I opened the starter code python file and saved it in matplotlib-challenges folder. I pushed changes to my repo on github via gitbash using git add ., git commit -m "", git push.

For both part I, "weatherpy." and part II, "vacationpy," I used Jupyter Notebook to record the code and run the code. The starter codes for both parts included the dependencies/set-up. For weatherpy I xx.... For the vacationpy I imported the csv file I created in the part I. 

The highlights in both parts were xx.

I made sure to keep the main data frame untouched so I could call it at anytime I needed additional data but I also created a demographic speicfic data frame so that I could call only the data that was age and gender specific.

The code for the scatter plot that includes the line equation (using the annotate function) is this:

line_eq = "y = " + str(round(slope,2)) + "x + " + str(round(intercept,2)) plt.scatter(Cap_tum_avg['Weight (g)'],Cap_tum_avg['Tumor Volume (mm3)']) plt.plot(Cap_tum_avg['Weight (g)'],fit, "r-") plt.title('Mouse Weight Versus Average Tumor Volume') plt.annotate(line_eq,(18,36), fontsize=15, color="red") plt.xlabel('Weight (g)') plt.ylabel('Averag Tumor Volume (mm3)') print(f"The r-squared is: {rvalue**2}") plt.show()

I cacluated the correlation coefficient using the following:

correlation = round(stats.pearsonr(Cap_tum_avg['Weight (g)'],Cap_tum_avg['Tumor Volume (mm3)'])[0],2)

Finally, I used the following to calculate the linear regression:

slope, intercept, rvalue, pvalue, std_err = stats.linregress(Cap_tum_avg['Weight (g)'],Cap_tum_avg['Tumor Volume (mm3)'])