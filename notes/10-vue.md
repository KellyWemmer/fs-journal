# MVC

8/15/22
if reading docs use vue3
vue github page

vue starter

npm i after new project

components automatically registered

No controllers folders

router.js - new pages

starter template localhost8080

app.vue - html template
    cntrl s

    script section
        new controller
    Appstate
        no classes/proxystate
        exports reactive
            computed = proxystate.on


app.view
    template-hello world

appstate
    enemy

create model enemy
    enemy: NewEnemy in Appstate

app.vue
    enemy: computed
    double curlies on 100 - add enemy.health in curlyboys
    <!-- <img src- use colon to bind enemy img -->
    @click in app.vue
    slap fx
    attack fx
    disable buttons if 0

enemy model do getter

v-if, v-else in app.vue
change text colors

attacks array in appstate
new model attack
    replace buttons app.vue - attackButton

components attackButton.vue
    template 
    script tag - props:
props are important

style tag in attackButton

player model

accessing template but it's not in scipt
    common error

v-model form
use ref: for anything editable

8/16/22 movie api

axios service
movies service
movie model
Appstate
movie service getMoviesBy search
    use params when adding query parameters

start server/npm i

pages
    HomePage.vue
        delete template
        headers/footers come from app.vue
        delete default styling .home etc
        new template vt tab
            name class = which page it is

order of params doesn't matter for query

homePage
    movies: computed
    {{movies}} to show up on page
only write code in setup function
    use return when users have to interact with
    setup = private

button in template
    get raw data

MovieCard.js

HomePage
    v-for
        key=if this movie changes, update this one element, don't need to redraw all movies
    MovieCard - needs to be same spelling as component MovieCard.js
    key will always singular "m" in movies + id
    :move = "m"

prop:
    movie: type, required true
    props needs to match movieCard
        props do not need to be returned

HomePage.vue
    use lifecycle hooks to load page
    onMounted -  need to import
        run fx getMovies
        don't have access to getMovies in return
        move to private

don't write forms in homepage
    searchform.vue
    form
    searchMovies fx
    v-model = "query"

setup
    const query = ref('')

need to return query

modal component
    don't need to target id's
    can use tag slot
    put modal in moviecard

data-bs-target on image

instead - make active movie for modal

app.vue
    Modal

appstate
    activeMovie
    v-if = 'activeMovie'

app.vue
    computed activemovie

movieCard
    bs - targe = #active-movie
    @click

can setactive movie in service

modal component delete header/buttons

homePage activeMovie
    button add to watch list

create array in appstate for watchlist
fx loadstate

MovieService addmovie to watchlist


Router
    router.js
    add new page

pages
    addWatchlistpage.vue
    default template
    can access by /watchlist in browser

nav bar
    add watchlist

add html to watchlistpage
    movies computed

movieservice
    res.data.page

8/16/22 Fireside Pokedex Vue
set up view
    app.vue
    main container fluid html

axios service
PokemonService getPokemon

homepage onmounted

log the getApi and console log

render raw data
add button
use v-for drawing name to button

use ? before name to wait for data

button setActive - url

console log active pokemon
html for active poke

use elvis operator if doesn't read page yet

Pagination
next in console results = next page url

create next/previous buttons

get request in PokeService
    nextpage and previous page in appstate
    appstate pages = null
    log in console - check we have correct pages

HomePage @click change page
computed next page and prev page
changePage() Home Page/Service
look at offsets to see page in console

previousPage
    disable button when !previous
height and weight still on page
    v-if = active



            