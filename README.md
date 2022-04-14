# HTTP / Crud Project

## Objective of Project
- Desmonstrate understanding post, put and delete HTTP methods and how to make them interact with server data.
- Demonstrate understanding of how to sync server data with an applications internal state.
- Use Routes to pass values to component to properly update the updating the state.

![Movie DB Example](project-use.gif)

## Instructions
### Task 1: Project Set Up
* [ ] Create a forked copy of this project.
* [ ] Clone your OWN version of the repository in your terminal
* [ ] cd into the project base directory `cd web-module-project-HTTP`
* [ ] Download server dependencies by running `npm install`
* [ ] Run the local web server by running `node server.js`
* [ ] Open a new terminal window and cd into the client code `cd client`
* [ ] Download project dependencies by running `npm install`
* [ ] Start up the app using `npm start`

## Project Features 
#### Editing a Movie

#### Deleting a Movie

#### Adding a Movie

### Adding in the Future
- Make the added DeleteMovieModal appear and be reacted to before deletion occurs.
- Add in `addToFavorites` functionality. When the favorite button is pushed in the `Movie` component, make sure that when the favorite button is pushed, the id and name of the currently viewed into the favorite state slice in `App.js.`


### Resource: API documentation 
#### GET `http://localhost:5000/api/movies`
- Retrieves all the Movies with the following formatting:
```
[{
  id: 5,
  title: 'Tombstone',
  director: 'George P. Cosmatos',
  metascore: 89,
  genre: "Drama",
  description: : "A successful lawman's plans to retire anonymously in Tombstone, Arizona are disrupted by the kind of outlaws he was famous for eliminating."
}]
```
#### GET `http://localhost:5000/api/movies`
- Retrieves all movies on the server.

#### GET `http://localhost:5000/api/movies/:id`
- Retrieves a movie with the passed value as id.

#### POST `http://localhost:5000/api/movies`
- Adds the movie passed in through body to the server movies list. Returns updated movies list.

#### PUT `http://localhost:5000/api/movies/:id`
- Replaced the movie with the passed in id with data passed in through body. Returns update movies list.

#### DELETE `http://localhost:5000/api/movies/:id`
- Removed movie with the passed in id. Returns the deleted movie's id.