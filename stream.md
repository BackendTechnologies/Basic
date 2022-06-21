## Readline  

https://nodejs.org/api/readline.html  

The **node:readline module** provides an interface for reading data from a Readable stream (such as process.stdin) one line at a time.  
**Readline Module** in Node.js allows the reading of input stream line by line



## Stream  

Стримы - это удобный(абстрактный) интерфейс для работы с потоковыми данными  
**Streams** - is a convinient unified programming interface for reading or writing data, sockets, and transferring data between process  

streams were invented before node.js
стримы это общая концепция программирования

file:///E:/Programming/Node.JS_course/Movies/Node.js/32/lesson.pdf


### Advanages  

- separation of concerns  
(стримы это инструмент который позволяет создавать маленькие компоненты, которые делают что-то одно и очень хорошо, например мы можем  
изменять код отдельного стримы, что позволит лучше управлять нашим приложением).
- flexability  
(стримы очень гибкие, их можно легко подключать, перенаправлять мы можем направлять данные из одного источника в множества других пунктов назначения.)  
- memory and time efficency(fs.readFile)  
Например есть файл 3 гига и для того чтобы считать его целиком нам надо 3 свободных гига, если их нету то процесс скорее все крашнется и  
мы не сможем  раюотать с такими фйлами, стримы за счёт того что они оплучают данные  по кусочкам тем самым потребляют небольшое кол-во памяти и равномерно
так как поток который идёт через стрим равномерный  
эффективность по времени заключается в том что мы можем работать с данными сразу если это стрим, не надо ждать пока видио запуститься полностью

### Виды стримов

Readable  
Writable  
Duplex
Transform  (вычисляют на основе входных данных некие выходные данные и отдавать их дальше)

### Data that sreams work with  

Buffers(or strings)  
Objects

**Buffers - это такие объекты которые нужны для представления данных фиксированной длинны**  

![Screenshot_1](https://user-images.githubusercontent.com/66359081/174751427-5e24df89-384d-4bec-895f-3c8b71ad9d48.png)

**All streams use internal buffers to store data

Writable streams inherit from stream.writable class.  
instances of writable stream provide 2 main methods for writing data:  
writable.write and writable.end  
Writable streams use eventemitter api. list of events: error, drain, close, finish, pipe, unpipe  





