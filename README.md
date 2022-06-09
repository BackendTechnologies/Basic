# Basic

## npm

node package manager

Прротокол описыает как фронтенд общается с бэкэндом.

Example: frontennd sends http request with data which describes what it need from backend and backend sends response.

Protocol describes rules in this case how they will interacts.

**require** - is global function which acsses from any place in node.js and it takes string

В devDependencies - зависимости для  удобной работы, для разработки 
В dependencies - заавимсоти без которых приложение не будет работать

**--save dev**  equals -D save in devDependencies
**--save** equals -S save in dependencies

**--production**

версии зависимойстей: major, minor(баги), path(не влияет на работу пакета)

**history** - get all commands which we enter in a field  
we can use **!id** for enter some commant that we need

**node.js** consists from different modules and libuv

**libuv** can work with operations system, create process, do http request, create flow, file system

**nvm** - allow use some versions of node js

find command in packet    
example: nvm -h |(pipe) rg install

Буффер - это представления наших даннных в бинарном виде(шестнадцатиричном).

EventLoop in Node.js has macroTasks and mikroTasks
It consists from demiptiplexer and queque that consists from 2 column(macroTasks and mikroTasks).

Aplication sens async task in the Event Demultiplexer  
Demultiplexer send this task in que (Event Queue) where we have special place for mikroTasks and  
anothe special place for macro tasks.
In the end when task will have implemented than eventLoop moves this task in the app. return result

makroTasks - setTimeout  
mikroTasks - promises




