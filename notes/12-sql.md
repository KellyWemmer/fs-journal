# MVC

ScaleGrid.io
Fly.io
On render
planetScale - has limitations
MySQLtutorial.org

dotnet-auth

sgroot
H_Ur7E1YEww0GIkH

open query
freebie.sql
create-db-template.sql
data

Create Table in freebie.sql
default characterset utf8;
primary key

bool - store as 1 or 0

once executed, do not execute again

Insert into

select from 

controllers,models, repos, 

public class CarsRepository
    GetAll
    private readonly IDBConnection _db
        comes from startup.cs file
        generate constructor

        string sql= @"
        Select * from cars;
        _db.Query<Car>(sql)
        "

dbSetup.sql for repo
execute

model
prop
no constructor needed in model

Startup.cs
    CarsRepository
    CarsService

Controller

Service sql
ExecuteScaler=execute code only once

9/15
dotnet vue

dbSetup
open query on database
accounts in dbSetup
env from appsettings
start servers
login
change to5001 server in env

create Table
comments-put comments in column names

create relation between  account and piece
    reduces orphan data
account id from account Table

Model,repo,service,controller,startup

get in controller
join in dbSetup
    in repo
    
    select everything from piece and account
keep tables in specific order 

add account to model

9/16

connect "ETIMEDOUT"

Many to Many

model for collectionpieces
new api controller
repo, service
    add to startup

collection controller
    
write sql in dbsetup first to test

collectionpieceviewmodel - extra id

9/19

new class Rep Item in Repo Item Model
createdAt in account

T - dataType we don't know yet
a generic

Make profile class so don't have to use account class

Interfaces
    Interfaces in service
    can call out properties and methods
    creates blueprint for what repo should have

9/20
.env, development, change localhost

cult model and repoItem

another public class profile

Cult extends Repo
profile has everything in profile plus whats in repoItem

9/21

view model in account
cultMemberId - relationship to cult
get list of accounts tied to cult
inject cultMemberServices

cultmemberservice delete for final

buttons fixed to bottom of modal

can't submit form if not completed

valid auth - logged
valid auth - no one logged in
invalid auth - logged in as someone else

do not have to edit on front end

