## Goodreads Analysis


This repository is dedicated to crawling and analyzing the data from social media [Goodreads](https://goodreads.com). Social Network analysis on the Users of the goodreads would provide us with a better understanding of the user's behavior in reading Books. 

### Crawling the Data

Goodread's Data is accessible through XML files. First You need to get your API key then The piece of code here will help you to makes requests to the API and save the Data from the XML file into CSV files.

Unfortunately the API doesn't provide us with the Number of Reviews and Ratings of each user, So we use Selenium to scrap the user profiles and get these data.

The user's ID is used to access the books he/she listed as **READ BOOKS**, and the Book's ID is used to gather the Data of the Book's Author. By making some minor changes, we can also access the **Currently-Reading** or **To-Read**. The code generates 2 CSV files.

User profile CSV file: 

- Userid
- Name
- Gender
- Location
- Rating
- Review
- Joined-Data
- Shelves_count
- About
- Image_url

User Books CSV file:

- Userid
- Book
- Publish_year
- Rating
- Rating_count
- Description
- User_book_review
- Author
- Author_id

The Only limitation in crawling data from Goodreads is time. The service doesn't let developers make requests in less than 1 seconds each time, this can be solved by running the code in parallel. Crawling 1000 users data with this method takes almost 5 hours. 

### Social Network Analysis on the Books and the Users

To be added soon. 
