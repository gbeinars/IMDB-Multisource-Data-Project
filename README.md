# IMDB-Multisource-Data-Project

<p align="center"><project-description></p>
This project used multiple sources, including a flat file, csv format, website data, and pulling data from an API. Ultimately, the data was cleaned individually, merged and stored in a database.

Included in this repository are data, milestones completed, and final presentation.

### Summary
In order to complete this project, I had to learn many techniques that I previously thought of as intimidating. The most difficult was surprisingly finding data sets of three different sources. There is so much out there with potential, and without knowing exactly how I would be transforming these in the future made it tricky. I ended up going through three different APIs before deciding the one that would work best with my project.

I focused on movies and IMDb ratings, specifically, but also explored genres, movie years, and movie rating (PG, R, etc.). I started with a CSV file where I did some cleansing, including visualizations, in order to identify any outliers. Due to the extensive amount of data in this file, I chose to remove rows with missing values in the columns that I would be focusing on. The remaining columns that had missing variables, I substituted with zero. Some column header formatting was required, and in the end, the CSV file was a clean dataframe.

To clean and format the website, I used the BeautifulSoup library. I used the exercises in the book to obtain the data from a website and transform the table from html into a dataframe. Some additional formatting and cleansing was required, such as splitting columns, dropping columns and removing parenthesis around each ‘year’ observation after splitting. This dataframe required the most cleansing and transformation of them all. I was pleased with the outcome.

Connecting to the API in order to pull the data was more challenging than the previous tasks. I used tthe titles in my dataframe from the website file to pull data from the API. I created a loop so that each title of the website movies was pulled from the API and added to the list. Then I used the list to create a dataframe. I was able to obtain additional information on each film from the website milestone. Similar transformations and formatting were required to clean the dataset.

Finally, I used sqlite 3 library to create a database, and add each dataframe as a separate table. I used a loop to show me the first 5 rows in order to check that each table was added correctly. Then I used JOIN to merge the tables on the primary key of title. Once converting the joined tables to a dataframe, I created multiple visualizations to represent the cleansed data.

## Links
[IMDB Top 250] (IMDb Top 250 - IMDb.html)</p>
[API Service URL](http://www.omdbapi.com/?)</p>

## Built With

- Python

## Future Updates
N/A

## Author

**Gabrielle Beinars**

- [Profile](https://github.com/gbeinars "Gabrielle Beinars")
- [Email](mailto:gbeinars@gmail.com?subject=Hi "Hi!")
- [Website](https://gbeinars.wixsite.com/my-site)

## 🤝 Support

Contributions, issues, and feature requests are welcome!
