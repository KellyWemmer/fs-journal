# MVC

8/8/22

bcw-create
node server

don't open node_module

.env
    do not push to github

play button on vs code
    start server
    server running on 3000
    type in local host in browser api/values

Controller
    basecontroller - handles errors
        inheritance

        super - lables mount path or "door"
        router and http requests

export class extends baseController
constructor - ets error
    always have to put super call if controller is extend

    this.router
        .get - runs fx

async fx, use.logger.error (utilities)
    use req, res, next as parameters

service

create fake db

controller
    res.send(cats) to send response

reload server every time change info on server

home, workspace
    makes requests

raw data JSON

get /:catId, this.getCatById

open play button, click on line that needs a breakpoint

editcats

8/9/22

copy code from server/models values
paste into new model
    change valueSchema
    keep timestamps etch
        make: string, required
        can put form requirements here
        put maxlengths on strings
        types: num, use min:
        img type: string maxlength 600

        mongoose/docs/api/schema has what you can put in a schema

export schema for DBContext
    register cars = mongoose.model

CarsController
CarsService
    let cars- async dbContext.Cars.find({}) --query object
    return

    Change password in mongo security database users update user

localhost3000/api/cars in browser

CarsController 
    get by ID, post, delete, put

postman
    api/cars

can go to mongo database
    can update database, but don't

Express library on top of nodejs

Startup.js
    Registers all controllers in controllers folder

F5 respin server

last week's gregslist 
change baseURL to localhost3000

can click and drag controllers
index.html redo ID's
do not drag main.js-retype

Cars Service-need to put API

Import controllers from correct location

8/10/22

NoSQL - document databases
SQL

model

assignment schema
    put "Course" in dbContext as magic string

register assignments in dbContext

controller/service

command 
    cat .env

assignments controller/service

postman
    create assignment

get course assignments - in courses controller, not assignments

in assignmentservice
    find courseId-matches model
    property name and value

find requires curly boys

enrollment model
    add courseID and virtuals

.use - middleware
    need to through auth0 to get info
    is positional

localhost3000 login










