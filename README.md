This is an application to store repositories in your portfolio, which will allow you to create, list, update and remove the repositories, and also allow the repositories to receive "likes".

[Video explaining how the project was developed - in Portuguese](https://www.youtube.com/watch?v=beeGtGzx9eA&t=105s)

## Requirements to run the application

  - [Node.js](https://nodejs.org/)
  - [Yarn](https://yarnpkg.com/)

## To use the project

1) You can download the project through the zip: https://github.com/joseaugustodardengo/GoStack-Challenge2/archive/master.zip or by cloning the repository https://github.com/joseaugustodardengo/GoStack-Challenge2.git
2) Access the folder where you saved the files and run the command below to run the project. Esse comando ira criar a nossa aplicação criando um container da nossa aplicação
```sh
yarn
```

## Application routes
* The application runs on http://localhost/3333
* ```/repositories -> using the POST method on that route will create a repository ``` 
* ```/repositories -> using the GET method on that route will list all repositories ```
* ```/repositories/1 -> using the PUT method on that route will update a repository according to the id that was informed. The route should only change the title, url and techs.```
* ```/repositories/1 -> using the DELETE method on that route will delete a repository according to the id that was informed```
* ``` /repositories/1/like -> using the POST method on that route will add likes to the specific repository chosen through the id```

## Example of using routes
The route POST received the following elements on the **request body**. In this route, **always** start 'likes' with *zero* value
```js
    {
    	"title":"Chanllenge 2",
    	"url":"https://github.com/joseaugustodardengo/GoStack-Challenge2",
    	"techs": ["NodeJs","Javascript", "Java"]
    }
```
The output on the screen
```js
    {   
        "id": "885dede8-b009-428e-8c39-d661977129a3",
    	"title":"Chanllenge 2",
    	"url":"https://github.com/joseaugustodardengo/GoStack-Challenge2",
    	"techs": ["NodeJs","Javascript", "Java"],
    	"likes": 0
    }
```

### Techs used
* [Node.js](https://nodejs.org/en/)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Express](https://expressjs.com/)
* [Nodemon](https://nodemon.io/)
