# Basic

## npm

node package manager

Прротокол описыает как фронтенд общается с бэкэндом.

Example: frontennd sends http request with data which describes what it need from backend and backend sends response.

Protocol describes rules in this case how they will interacts.

**require** - is global function which acsses from any place in node.js and it takes string

В devDependencies - зависимости для  удобной работы, для разработки 
В dependencies - заавимсоти без которых приложение не будет работать

**--save-dev**  equals -D save in devDependencies
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


**Node js многопоточный?**  
Да и нет
![Screenshot_3](https://user-images.githubusercontent.com/66359081/172872158-06be9bb0-1f8c-43c0-9478-60ac0f737e3e.png)

процесс - это область  памяти которая выделяется для работы какой-то программы

**require**  
![Screenshot_4](https://user-images.githubusercontent.com/66359081/172889772-bad5a88b-c28c-4693-94e0-7d8ff5d364b2.png)

**commonJS** интегрировали в Node.js(там есть require)


**module** - 

Pattern module 
![Screenshot_5](https://user-images.githubusercontent.com/66359081/172891225-2cb0ac02-a884-4d16-be5f-3ef19822ed2d.png)
Оборачиваем в самовызывающую функцию чтобы сделать scope


**barrel file** - one file re-exports another files  
![Screenshot_6](https://user-images.githubusercontent.com/66359081/172895716-f7981e05-6191-47ca-93c2-8627a50a1bb0.png)

**кэширование** - каждый модуль импортируется один раз и сохраняется в кэш зависимости(кэши).

**Буфер**(в целом) - это представление файла(любого) в бинарном виде.  
**Буфер**(в js) -  
длина не изменяетс, значения можно изменять

```js
057
47 - восьмеричная


058
58 - десятиричная
```
разные системы счисления

1 bite = 8 bit

чекнуть значение в бинарном виде  
(7).toString(2)  
111

192.168.158.19  - IPV4
4 bit
максимум  число 255 можно представить в 1 bite
4 млрд портов

в терминале будет в 16-ой системе счисления

**кодировка** - представляет собой таблицу, где каждый символ имеет свой порядковый номер(ключ: значение)


### Переменные окружения  

относятся не к node.js а к опер системам  









