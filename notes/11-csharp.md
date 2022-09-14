# MVC

render
sign in with github
get started for free
new
web service
configure account if needed
connect
build command
    don't open in workspace vs code
    package.json
    copy paste build command and start command

advanced
    enviro variables
        connection string and auth0 from .env - server

copy url go to auth0
log into website
    paste into origins

vite.config.js
outDir: server/client
    if have a server
    npm run build
    commit

mkdir 
dotnet new console -n (name)

DataTypes
string
char
int
float
double
decimal
bool
arrays - have to be same DataTypes
lists<subdatatype> uses .count
dictionary<key, value>

constructor
    public method of same name of class

9/13/22

bcw create
dotnet auth
do not use hiphens or hashtags in name for dotnet

appsettings - like .env

model
Cat.CS
namespace
public class

use C# for visual studio code and C# extensions 
    use shortcut prop

catscontroller.CS
namespace
public Cat - datatype GetCat()
    return new Cat
    public actionresult with a cat inside GetCat()

constructor in model
    public Cat
    Cat control.

browser hit advanced
    continue to local host unsafe
    get cat 

add CatsService

repositories
    create fake repository
    build constructor

CatsService

Startup
    line 38/39
    register our service and repository
    create singleton with AddTransient

Controller DELETE

? for Lives
    Lives are either null or int Lives

