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




