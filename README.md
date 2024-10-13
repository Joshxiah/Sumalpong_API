Project Title
# Sumalpong_API
Description
## Description
This is a simple Express API for managing a collection of movies. It allows users to perform basic CRUD (Create, Read, Update, Delete) operations on a movie database, with data stored in a MySQL database.
Installation Instructions
cd movie-api
Usage Instructions
node server.js

API Endpoints :
1. Get All Movies
Endpoint: GET /movies
Description: Returns a list of all movies.
2. Get a Single Movie by ID
Endpoint: GET /movies/:id
Description: Returns a single movie by its ID. If not found, returns a 404 error.
3. Create a New Movie
Endpoint: POST /movies
Description: Creates a new movie. Requires title, director, year, and genre.
Request Body:
json
Copy code
{
  "title": "Movie Title",
  "director": "Director Name",
  "year": 2024,
  "genre": "Action"
}
Response: Returns the created movie with its auto-generated ID.
4. Update an Existing Movie
Endpoint: PUT /movies/:id
Description: Updates an existing movie by its ID. If not found, returns a 404 error.
Request Body: Include fields you want to update.
5. Delete a Movie
Endpoint: DELETE /movies/:id
Description: Deletes a movie by its ID. If not found, returns a 404 error.
