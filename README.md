# movielist
 This is a Python web application using Flask, a popular web framework, to create a movie rating and review system. The app allows users to add, rate, review, and delete movies. It also retrieves movie data from an external API, specifically "The Movie Database" (TMDb), to populate the movie information.

Here's a brief description of the main functionalities of the application:

Home Page ("/"): Displays a list of all movies in the database, sorted by their ratings. Each movie is shown with its title, release year, description, rating, and an image poster.

Add Movie Page ("/add"): Provides a form where users can enter the title of a movie they want to add. After submitting the form, the app sends a request to the TMDb API to search for movies with the given title. The API responds with a list of movies matching the search query. The user can then select the correct movie from the list to add it to the database.

Find Movie Page ("/find"): When a movie is selected from the list on the "/add" page, the app retrieves more detailed information about the movie from TMDb and adds it to the local database. The movie's title, release year, description, and poster image URL are stored.

Rate Movie Page ("/edit"): Allows users to rate and review a movie they have added. Users can enter their rating out of 10 and add a review comment. The rating and review data are stored in the database for the respective movie.

Delete Movie Page ("/delete"): Enables users to delete a movie from the database. When a movie is deleted, it is removed from the list of movies on the home page.

The application uses Flask-WTF for handling forms, Flask-SQLAlchemy for database operations (SQLite is used here), and Flask-Bootstrap for styling and layout. The movie data is retrieved from TMDb using their API, and movie posters are displayed using image URLs from the API.

Please note that for the application to work correctly, you would need to sign up on the TMDb website to obtain an API key and replace the "Your API Key" placeholder in the code with your actual API key. Additionally, this description assumes the TMDb API structure and endpoints have not changed since the model's knowledge cutoff date in September 2021. If there have been any changes, the code may need to be updated accordingly.
