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