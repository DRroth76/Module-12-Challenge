# Module-12-Challenge
NOSQL_setup_dr
In this challenge, I imported the 'uk_food' database using mongoimport. From here I wrote code to see if the 'uk_food' database was amongst the databases that I have created before.
I wanted to see what collections were present, in which case only the 'establishments' collection was.
I saw what a document in the collection looked like using pretty print, and then I set the collection to a variable name.
Using code provided for us in the challenge webpage, I created a new establishment document with the name 'Penang Flavours' and inserted it into the database, and sought to update BusinessType with the id that corresponding to the 'Restaurant/Cafe/Canteen' type.
I then deleted every document with the LocalAuthorityName of 'Dover'.
Then I changed the datatype of latitude and longitude for each document into a double, and the RatingValue to an integer, weeding out any nonnumeric values.

NOSQL_analysis_dr
I repeated the same steps before to plug into the 'uk_food' database that I created before, along with the 'establishments' collection.
My first analysis looked for establishments that had a hygiene score equal to 20. There were 41 establishments that fit this criterion. With this information I created a DataFrame with 10 rows visible.
My next analysis looked for establishments that had a LocalAuthorityName of London, as well as a RatingValue of 4 or higher. 33 establishments fit this criteria. I used the regex function to look for any LocalAuthorityName with 'London' in the string value.
I created a DataFrame here for this, with 10 rows visible.
My third analysis looked for establishments that were within 0.01 degree latitude and 0.01 degree longitude of my created establishment 'Penang Flavours'. Additionally, they must each have a RatingValue of 5.
I then sorted the documents by hygiene score in ascending order. This too was made into a DataFrame with the top 5 rows visible.
For my fourth and final analysis, I wanted to find how many establishments for each LocalAuthorityName had a hygiene score of 0, wanting to sort by count in descending order.
As has been done before, I made a DataFrame for this analysis. Thanet, with 1130, have more establishments with a hygiene score of 0 than any LocalAuthorityName, followed by Greenwich, Maidstone, Newham, and Swale.

My files are labeled with 'dr' because of my initials.
