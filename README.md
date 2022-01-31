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



# Endnote

This crawler crawls hotel information in Seattle, but only including checking in on February 13, 2022, and checking out on February 14, 2022. However, adjusting the time frame would not be easy, the url of the Expedia website is hard to parse. 



