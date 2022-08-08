# MVC

8/2/22

bcw-sandbox.herokuapp.com/api/cars

need to keep property names from servers

html title
axios library script

make sure descriptions are similar for server
add id to constructor

Make axiosservice.js
    export const api = axios.create...
    can add timeout

delete stuff in carservice


createCar function
    debug

create carin controller
    debug

create car in form

step through
    img does not match server

goes to car service
    will have id wen receives from server
    update new object in service
    need update img in controller and model

async try catch in controllers for createCar

createCar in service
    after importing axiosService
    can use api.post ...
    res.data - data is the response from server
        if not sure of response name, use debugger or in network

fill form
    rendered to page

delete cars in appstate
edit localstorage
    should hae been in service

carservice in constructor

get cars in carservice

add trycatch to cars controllera

viewCars
    getCars

rest
    url api/(resource - pluralword)(id)

deleteCar in services

F2 change all names

editing 
    when edit=begin to edit
        need previous data to edit

try catch always in controllers

create folder
    Components
        file carform.js
        export function getCarForm()
        ext es6stringhtml tobermory html highlight

getCarForm and return

carsController drawCars
    getElement by ID form = getCrForm()

carForm
    set value for interpolation on html
    sets form to undefined
    change to empty string/0

get CarForm
    new car

add edit button with onclick

cars controller
    do not use async
    adjustCar()
        finds the car and change form

need to find id to edit
if statement in car form
edit car in controller

editCar in service

gets and deletes - do not send data
    do not use commas

8/3/22

3 controllers
3 services
    activeSpell is part of dndcontroller
Models
3 models

create models and classes
    export classes move to new file

main.js

services create with axiosservice
    export api's for for each sandbox and dnd

dnd spellservice export and sandox export

appstate
    activespell = null or empty object
        only have 1 active spell at a time

sandbox/name/spells

dndapi/spells

active spell when clicked url

html
    main/container
    rows/columns
    id's

axiosservice url

dndspellservice get spells

dndspell.js constructor and template

api already in url
change base url in axios service
add api to dndspellservice

dndcontroller
    constructor
    drawspells

selectable no-select to remove highlight

setActiveSpell in dnd Controller

spellservice
    url is it's own object


create template in activespell

style.css
    left pane scroll

activeController
    draw-not iterating  over array

activespell.js
    don't need parameter in onclick because only one spell in proxy

sandbox controller

sandbox spell
    extend activespell
        super data fills out in activespell nd then continue to add
        id and prepared
        data is added to activespell parameter

sandboxspell service

add sandbox url to axiosservice

error because description was array instead of string

activeSpell 
    data.desc.join

draw in sandbox controller

add known spells to html and sandbox controller

sandbox model
use terniary

when check box
    onchange

sandbox controller fx
sandboxservice

needs equal sign in proxy state

8/4/22

get data in console
    make playerscontroller
        export class log constructor

        main.js

        check console
set up axiosservice
    export const 
    baseURL capitalized
set up script tag

get object from api to test in browser

copy to baseurl
timeout

export sandbox
    baseurl and sandbox

playerscontroller
    getPlayers()
    await players serive

create Playersservice and export const

controller

service getPlayers and log res.data
    this.getPlayers calls function as soon as page loads
    ProxyState.on

data logged onto console

Create model singular
    export class
        shift alt down copy's down
        ctrl D

Go to Appstate and import

Service
    ProxyStateplayers res.data.map

register listener in controller for players
    draw fx
    log players

template in player js (button)

html 28

copy to playertemplate

players controller
    let template
    id

Set Active Players
can use players controller
    is not new url address

Appstate empty object
    singular vs plural

controller for player in playerscontroller

drawPlayer singular

id on player-name and playerscore

singular drawPlayer fx
    if statement for if no player

player model onclick

controller
    set active player, make sure id is in service too

console.log for id's

name and points rendered

new Clues controller
    log

main.js

async getclues()

new CluesService and class/export

service
    CluesService
    console log getClues to test
        make proxystate for getClues

if statement in getClues


test event listener

Reset "stage"
clue model export class

console.log right click property path

html another template

paste in clue template

set up players in appstate

clueService getClues()

ProxyState for clues
drawClues

query random?

set params inside get
console request URL in network

modal bootstrap
    modal under footer in html
    change id's
    copy button
    change id of button
        paste in clueTemplate?

onclick on cartemplate

setActiveClue in controller and service

listener in cluesController
    drawClue in cluesController
    log

format html for question/answer
    paste in clue.js

    on-hover, will work on parent class

getId for drawClue in Controller

data-bs-dismiss will close modal

change/edit buttons
    onclicks on icons

answerQuestion in contoller
    declare in service
Target listener else answered


Fireside

forms
checkboxes
post put delete get
toggle
dynamically changing css
MVC
moonminer interval

html-remove junk
div id's
creat controller and servicce for each id

players controller

string interpolation for css
    need hashtag for hex codes
    need to see style in console

user will be set to YOURNAME
need new image on reload
temp in kelvin
    will need convert
    toggle between c/f

already randomizes images and quotes

icons for weather in open weathermap

NEED COUNTS FOR TO DO'S





