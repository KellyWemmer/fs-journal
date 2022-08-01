# MVC

7/25/22
model view controller
    keeps data clean and structured

View
    index.html
    what user sees
    links to main.js
    type=module

Controller
    .js
    interface (go between) for the user
    connects to service.js

Service
    Service.js
    the business logic
    performs the function

AppState
    place that holds all the data
    single javascript
    holds models

Model
    a format for which the data will be saved
    what the data looks like
    a class,

view to controller to Service 

In hero.js
    class Hero --needs to be Capitalized

    constructor(name, health, etc) --used to build hero, needs properties
        "this" only refers to each current hero

    need to 'export'

import {Hero} from 'hero.js'

in js
    let  heros

cannot read console before model has been built

if a function is private, is not included in class bundle
    can call it from inside the class

get = function that has return and can be accessed by property

get random numbers and add margin to the race tracks

7/26/22

after loaded
remove line 29 in html
comment out controller instance

start with model and html
Dino class needs constructor - use for starting values
weight or not specified needs to be at end


Then appstate
    move @type above array of dinos
    make dino array/import Dinosaur.js

create controller for Dino
    constructor and console log it
        instantiate in main js dinoController = new DinosController()
    controller should load

make _drawDinos() private outside of controller class
    print dinos from AppState - has a proxy state - only allows access to dinos
        let dinos = ProxyState.dinos and log
    make template for dinos-keep simple and small at first to check for drawing

create get template in dinosaur.js and change this.name etc
can make controller template equal d.Template

 function hunger and updateDinos
 feed method
    service.feedDino(name)   
    controller does not do this function

    create class in DinoService and export const of class
        const - keeps dino service from changing and cannot be overwritten
        in controller
            dinoService.feed(name)

    log feed(name) does not exist
        need app.dinocontroller in template in dinosaur.js?
            app from main.js

find name in DinoService
and log
hunger+=15

put updateDinos in fee function in Controller

if statements for status in services

money function in Controller

make money function in dinoservice
put money in html


style.css in assets

7/27/22

get dummy cards before user generated content

main, take out controllers

start with models and export class
    constructor with parameters with "this"
    get simple Template with p-tags to test to page

Appstate
    change @type
    add array with 'new' items-keep simple to test

Controller export class
    constructor and log-

Main.js
instantiate controller in main.js

controller drawCars
    create template and draw c.template
    put in instructor for when page loads
    load template to console
    get elementID = template

html
    make id for attaching, console log in controller

html
    create templates
        don't use card
        selectable class

car.js
    paste template to get Template
    interpolate

html
    section form
    form tag
        has event
            onsubmit="app.carsController.createCar()
    submit button inside the form type=submit

write method in controller to create car
    log
        refreshes page as default
    window.event.preventDefault() to stop refresh on submit

html input field

controller
    log window event target 
        html should show up on console
    create variable for target
    console log(variable)

input type- put id and name in html
    now can log console.log(form.make.value) .make is the input (name)
    input rest of html (labels)for model,price etc and text area
    can put min for price

Controller
    variables = form.year.price etc

Service
    class CarsService
    export const carsService ...
    let newCar = {
        mke: form.make.value etc..
    }
    fx createCare(newCar) and log
    push to AppState
    drawCars() after createCar in Controller
        was undefined-did not have template
        need to turn into car in service

service
    push new Car()

put curly boys around parameters in cars.js
put curly boys and make, model etc in cars array in appstate

create listener or observer
    can replace drawCars with listener
    register the listener
        carsController
            ProxyState.on('cars', _drawCars)

appstate
    target.emit in set

service
    replace 'push' in createCar
        ProxyState.cars =[...ProxyState.cars, new Car(newCar)] ...spread operator

car template
    delete button

controller
    delete car fx and log

cars.js
    add id to object

utils
    generate ID
        use for template Id
        import generateID for Utils....

cars 
    interpolate id into template

service delete car()
    c.id == id, log
    splice, log
    need = sign to trigger proxyState to draw
        easier method
            proxystate.cars = proxystate.cars.filter( c.id DOES NOT = id)


add function to controller

controller
    form.reset under createCar

create localStorage.js in utils
    don't need to bundle

    export fx saveState() {
        ...JSON stringify
        localStorage...
    }

    export fx loadState() {

    }

Cars.js
    use proxy to update

console
    checked to save
    Application in cars-shows data saved in cars

localStorage
    parse rawData...
    and log

    when stringify, it loses it class

    proxyState.cars = carData.map(c = new Car(c))

    github
        fork to my name
        code https copy
        cd into projects git clone and past URL

7/28/22

title is parent, items are children

start in Model
    export class
        constructor
    get Template and log simple template

Appstate
    @type and new array

functions for form
    change type in html
    use min and min-length

controller
    createParty fx and console log
    collect data and send to service
        will store in appstate

html-onsubmit 

on numbers on form submit
    parseInt()

Controller
    push to service
    proxystate
    log

create in service and log

to draw
    register listener in controller

save to local storage
    need to map to reform class

editParty fx
    onblur = to "unfocus" element in html
        blur-when something is off-clicked

controller
    class Item
        constructor
        partyId = data.partyId
            connects item to party

items array in Appstate

model
    data.id or generateID() to keep previous ID


get Template
    get Items, use filter for item.partyID == this.id
     put draw inside get Template
     has draw fx's for own items

use Pop for alert
    use async and await
    can pause code depending on result of pop results

    Pop.toast

sort by date
    use Date class

draw fx in controller
    .sort

get PartyTotal in model

