#Anime List App

## Setup
### Required
- MongoDB
- `anime_list_backend` app running on `localhost:3001`
  - https://github.com/danlyg/anime_list_backend

### Initialize
1. Make sure `localhost:3001` is running with `anime_list_backend`
2. `npm install`
3. `npm start`

## Tech
- React
- Redux

## API
### Anime Backend
- https://market.mashape.com/vikhyat/hummingbird-v1
- https://hummingbirdv1.p.mashape.com/anime/{id}
  - id: **[Number/Title]**
  - EX: http://hummingbird.me/api/v1/anime/bleach
  - DOCs: https://github.com/hummingbird-me/hummingbird
### List backend
- http://localhost:3001
  - `/anime-list` get all anime from the list
  - `/anime-list/new` create a new anime item
  - `/anime-list/:id`
    - GET a specific item using `_id`
    - PUT update a specific item using `_id`
    - DELETE a specific item

## Road Bumps
### Webpack
  - Setting up webpack dev server port and linking with express http server
### ES6
  - Spread operator `...`
    - It is experimental so it requires `stage-2` babel preset to use
