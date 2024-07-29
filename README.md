# nosql-challenge
In this project, a new repository called **nosql-challenge** was created and the repository was cloned. Jupyter notebook, starter files and the Resources folder, which contained **establishments.json**, were added to this folder. Changes were then pushed to GitHub.

The UK Food Standards Agency's evaluation data was used to help the magazine "Eat Safe, Love" evaluate establishments for future articles. The data was imported into a MongoDB database named **uk_food** and the collection named **establishments**. Libraries such as PyMongo and pprint were imported, and an instance of the Mongo Client was created.

The database setup involved listing all databases and collections to ensure that uk_food and establishments were correctly created. The find_one() method was used to display one document, confirming the data load.

A new halal restaurant named "Penang Flavours" was added to the database. The BusinessTypeID for "Restaurant/Cafe/Canteen" was found and updated for this new restaurant. Establishments in Dover were identified and removed from the database, with document counts checked before and after removal.

The database was updated to convert latitude and longitude values from strings to decimal numbers and RatingValue to integers. Exploratory analysis was conducted to answer specific questions for the magazine. Establishments with a hygiene score of 20 were identified, and establishments in London with a RatingValue of 4 or more were found.

The top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score, near "Penang Flavours" were identified. An aggregation pipeline was used to find how many establishments in each Local Authority area had a hygiene score of 0, sorted from highest to lowest. The results were converted to Pandas DataFrames and displayed for analysis.