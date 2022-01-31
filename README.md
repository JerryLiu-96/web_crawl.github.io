# Motivation of the Project

This crawler crawls hotel prices, weblinks, and ratings at Seattle from Expedia. We hope the crawl can help users in decision making of the booking.



# Variables

|    Field     |                         Description                          |
| :----------: | :----------------------------------------------------------: |
|  hotel_name  |                      The name of hotel.                      |
|  hotel_area  |              The area the hotel is located in.               |
| hotel_rating | The rating of the hotel (Excellent, Wonderful, Good,...,Average). |
| hotel_price  |           Lowest price of the available the hotel.           |
|  num_review  |           Number of the review the hotel received.           |
|  hotel_url   |              The weblink of the hotel homepage.              |
| hotel_score  |               The score of the hotel received.               |

We search the hotel checking in on February 13, 2022 and checking out on February 14, 2022. The selection results are filtered by adults 2 and we input "Seattle, Washington" in the location. 

In google Chrome inspector, we find the tag for each search return:
![image](https://user-images.githubusercontent.com/84870579/151801708-cb31fbdd-15fb-486d-b4c8-a8f4d0c9f0f9.png)

Since the tag in the Chrome inspector are different from what we get in python script, we cannot find the tag of our interest by highlighting in Chrome, we print the html source code and find tags here in python.
![image](https://user-images.githubusercontent.com/84870579/151800280-1a17211b-bcce-4561-ac1e-cbb1cfe3f73b.png)
![image](https://user-images.githubusercontent.com/84870579/151802070-53a55962-9e32-430f-a55c-ad1a7be8069c.png)


We use the code to crawl the information of our interests.
![image](https://user-images.githubusercontent.com/84870579/151801082-0a1b6f19-0cdb-44f7-9541-07d00090e805.png)

Then we store values of the variables into a dictionary named "row" and we create a dataframe to store all the "rows". The bot is put to a 5 seconds sleep to prevent the crawler from being disabled as a DDoS attack.
![image](https://user-images.githubusercontent.com/84870579/151802675-5653af1a-7470-405b-9eaa-363a23e767f1.png)

![image](https://user-images.githubusercontent.com/84870579/151801082-0a1b6f19-0cdb-44f7-9541-07d00090e805.png)



# Endnote

This crawler crawls hotel information in Seattle, but only including checking in on February 13, 2022, and checking out on February 14, 2022. However, adjusting the time frame would not be easy, the url of the Expedia website is hard to parse. 



