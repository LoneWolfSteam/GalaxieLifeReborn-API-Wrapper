# GalaxieLifeReborn-API-Wrapper
A simple NodeJS node module 


## Installation

`npm i galaxielifereborn-api-wrapper`

## Usage

- getUserProfile

Get a user profile

- getServerStatus

Get server status

- getAlliance

Get data of alliance

- getAllianceMember

Get all members of an alliance

- getTopChipsPlayers

Get the ranking of the biggest chips players

- getTopLevelPlayers

Get leaderboard of level players ranking


## Exemple 

```js
let GLR = require('galaxielifereborn-api-wrapper')

GLR.getTopLevelPlayers().then((data) =>{
    console.log(data) //Return leaderboard
}).catch((err) =>{
    console.log(err)
})

GLR.getUserProfile("IamUser").then((data) =>{
    console.log(data) //Return UserProfile
}).catch((err) =>{
    console.log(err)
})

GLR.getAlliance("IamAlliance").then((data) =>{
    console.log(data) //Return Alliance
}).catch((err) =>{
    console.log(err)
})
```
