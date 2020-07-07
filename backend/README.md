# Repository Manager
A simple application to store github repositories of your portfolio, that it will allow you to create, list, update and remove repositories. And also, it will allow you to give "likes" to repositories.

The app was build with Node.js and Express and it is part of Rocketseat bootcamp.

## Running
- Install all the dependencies: `yarn`
- Run in dev mode: `yarn dev`
- Run tests: `yarn test`

## Routes

### Create repository
All repositories are created with 0 like.

HTTP Method: `post`

Route: `/repositories`

Request body:
```json
{
	"title": "Repository title",
	"url": "https://github.com/repo-url",
	"techs": ["Node.js", "Express"]
}
```


### List repositories
HTTP Method: `get`

Route: `/repositories`


### Update repository
The update functionallity doesn't change likes.

HTTP Method: `put`

Route: `/repositories/:id`

Request body:
```json
{
	"title": "Repository title",
	"url": "https://github.com/repo-url",
	"techs": ["Node.js", "Express"]
}
```


### Delete repository
HTTP Method: `delete`

Route: `/repositories/:id`


### Update likes of the repository

HTTP Method: `post`

Route: `/repositories/:id/like`

---
Desenvolvido com :purple_heart: por [Marcelo Palmieri](https://www.linkedin.com/in/marcelo-palmieri)