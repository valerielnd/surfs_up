# surfs_up Analysis

## Project overview

Before investing in a surf and ice cream business on the isle of Oahu in Haiiwi, 
the principal investor W. Avy needs to determine if this kind of business is sustainable 
year-round. Using an SQLite database that stores the weather data observed 
for several years from 2010 to 2018.

The list of deliverables for the project is:

- Determine the Summary Statistics for June
- Determine the Summary Statistics for December
- A written report for the statistical analysis

## Resources

We are given access to an SQLite database that stores the weather data to realize the analysis.

- [hawaii.sqlite](https://github.com/valerielnd/surfs_up/blob/main/hawaii.sqlite)

We used Python libraries Pandas, Numpy, and sqlalchemy and Anaconda's Jupyter Notebook to do the analysis.

- [Challenge Analysis](https://github.com/valerielnd/surfs_up/blob/main/SurfsUp_Challenge.ipynb)


## Analysis results

### Determine the Summary Statistics for June

To provide investor W. Avy with an overview of June weather in Oahu, we computed statistical 
analysis such as the mean, standard deviation, minimum, and maximum. Those hard results 
will help determine trends in the data.

![june_statistics](https://github.com/valerielnd/surfs_up/blob/main/june_stats.png)

As we can see in the results obtained from the calculations of the mean, minimum, maximum, standard 
deviation and percentiles using the describe() function from Pandas, the temperature 
in June, the first summer month, is favorable to the surf and ice cream shop business. 

* 	The minimum temperature is 64 degrees, and the high temperature is 85 degrees. 

* 	The average temperature is approximately 75 degrees, and as the standard deviation is 
	about 3.2 degrees, there is not a wide variance between the temperatures observed each day 
	in June, and the statistical average and this value are reliable.

*	The temperature for the first quartile is 73, and the last quartile is 77 degrees which means 
	less than 25% of the temperatures observed are less than 73 degrees, and about 50% of the temperatures 
	observed are between 73 degrees and 77 degrees.
	

	
### Determine the Summary Statistics for December

To provide investor W. Avy with an overview of December weather in Oahu, we computed statistical 
analysis such as the mean, standard deviation, minimum, and maximum. 

![dec_statistics](https://github.com/valerielnd/surfs_up/blob/main/dec_stats.png)

As we can see in the results obtained from the calculations of the mean, minimum, maximum, standard 
deviation and percentiles using again the describe() function from Pandas module, the temperature 
in December, the first winter month, is favorable to the surf and ice cream shop business. 

* 	The minimum temperature is 56 degrees, and the high temperature is 83 degrees. 

* 	The average temperature is approximately 71 degrees, and as the standard deviation is about 3.7 degrees, 
	there is not a wide variance between the temperatures observed each day 
	in June, and the statistical average and this value are reliable.

*	The temperature for the first quartile is 69, and the last quartile is 74 degrees which means 
	less than 25% of the temperatures observed are less than 73 degrees and about 50% of the 
	temperatures observed are between 69 degrees and 74 degrees.



### Key differences in weather between June and December

* 	The minimum temperature in June is greater by 8 degrees than in December, and the maximum temperature in June 
	is greater by 2 degrees than in December.
	
*	The average temperature in June is greater by approximately 3.8 degrees than in December, while their standard 
	deviation is low, which suggests low variability around their averages.
	
*	The temperature for the first quartile is 73, and the last quartile is 77 degrees in June, while it is 69 and 74 
	degrees in December, which suggest that less than 25% of temperatures observed in
	June is less than 73 degrees, while it is less than 69 degrees in December. Also, 50% of the temperatures 
	observed are between 73 and 77 degrees in June, while they are between 69 and 74 degrees.
	
	
## Summary

To gather more weather data for June and December, we could design a query to retrieve the last 12 months 
precipitation data for those two months to check if, even though we get a favorable temperature in those months, 
the precipitation levels will not be a problem.

As it is essential to open the surf and ice cream business in an active station, we could design another query 
to find the temperature statistics for June and December in the most active station.
	 