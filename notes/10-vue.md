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

8/17/22 Gregslist

edit account-need to know!

drag models/services from gregslistAuth

copy/paste keys under socket
vue localhost8080
    getting data from local3000 api/cars

Proxy = Appstate

router
    carspage

CarsPage.vue

onmounted getCars

computed cars

navbar-replace about=cars

add jobs in router before navbar
CarCard component - paste model template
    remove columns in components

edit template
props car

CarsPage
    v-for
        render card to page

modal component - from flix

make active car in carservice

active car in appstate

return

modal to button tag

form on CarForm component
    replace value with v model
    script editable
    watchEffect - when using form for edit and create
    handlesubmit

v-models

can view car properties in console

data-bs-dismiss to close modal after update

deletecar in CarCard

setActivecar to empty object

router
    /cars/:carId

CarPage
    car card pasted

new page car doesn't come from prop

router-link CarCard
    params

v-if car in CarPage

log in
    manage account

account page

account-whoever is logged in

accounts page
need form to change account info

accountform.vue component

8/18/22

view profiles/edit account

sandbox api projects

Project.js
    put defaults in data

axiosService
    baseUrl sandbox
    auth keys

start server
    8080
    Login - new account
    can log in/manage account

account page - can edit own account - settings
Profile Page - what I choose to show

component accountform
    form v-model editable
    label visually hidden

account page
    account form

accountform
    const editable
    watchEffect
    editable
    handle Submit

accountService
    editAccount

account form

f2 = can change multiple names

style in accountPage

add coverImg and bio to accountmodel
form rendered to page

ProfilePage
    log hello

router
    profile/:profileId

*****8080 profile/testing*****

ProfilePage***
    const route = useRoute
    route.params

ProfilesService
    getProfileById

log - id from account
    profile info in log

Profile.js

appstate active profile

Profile.vue
    computed

ProfilePage
    {{profile}}
    build template

breaks when refresh - is null at first

profilePagae
    v-if - profile
    else 

    if bad id
        router.push

accountform
    editable
        router.push

ProfilePage
    bg Image/coverImg
    :style
    height

ProfilePage
    v-if profile.id == account.id
    account computed
    router-link Edit Account
        is button

app.vue
    delete header/footers
    write new template

app.vue
    router link Art Establishment to home link

Login.vue
    bind Title

Projectform component
    form @Submit
    const editable
    watchEffect

    editable
    handlesubmit

ProfilesService
    createProject
    editProject
    delete
    get

appstate
    projects
    activeproject

HomePage
    getProjects
    return computed projects
    {{projects}} to page

ProjectCard
props are singular


HomePage
    project card template
    print titles

    new Date to local date string
    img v-for

ProjectCard computed

HomePage
    Projectform
    finish project form

editables
props
router links
what small steps to take to log as I go
Next steps on Gregslist project?

ProjectCard
    v-if project.creator
    router link with params
    css

ProfilePage
    coverImg ||
    add height im src

    container in ProfilePage

    add computed projects
    profileProjects in Appstate

    getprojectsByCreatorId
    onMounted

ProjectService
    getprojectsByCreatorId

ProjectCard
    v-if for edit button
    account:
    Projectform
    toggleEdit

undraw.io
no delete or edit on other posts
update class for bios

has posts api
    likeId's

    do not need likes array

do not create class called ad
don't use word banner

different sizes of ads 

if logged in and likeing post, will like or unlike post - needs to update to correct number of likes
can't like posts if not logged in

do not need to edit posts
need to edit account
need to delete posts when logged in 

do all gets first
pagination required on homepage and posts

due post but handle like a put - use splice
1st gregslist is good reference

log in before leaving