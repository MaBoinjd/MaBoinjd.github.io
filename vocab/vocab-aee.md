---
title: Anthony, Erik, and Ethan Vocabulary
permalink: /vocab/aee
layout: default
---

[Back to vocab page](/vocab)
<br />
[Back to main page](/)

# Vocabulary
**Binary/Hexadecimal** - Binary is 0s and 1s that are used to do things in computers. Computers read 0s as off and 1s as on and use binary for everything. Hexadecimal binary is a base 16 system that is used for images. 
- Bit: one binary digit, 0 or 1/on or off
- Byte: 8 bits, basic unit of data
- Nibble: half of one byte; 4 bits 

![Binary and Hexadecimal](https://i.pinimg.com/originals/fa/3f/8b/fa3f8b032f1df211cfa5a226b973f0e8.jpg)

**Data/Procedural Abstraction** - Data abstraction is where you separate the logistics of the data from how it is represented. Procedural abstraction is where you separate the logistics of an action taken from how it is implemented into the code.

![Data Abstraction](https://www.tibco.com/sites/tibco/files/media_entity/2021-08/data-abstraction-layer-diagram.svg)

**Lossless vs. lossy compression** - Lossless compression reduces all loss of data and is best used when you want to preserve the original data. Lossy compression loses some data but is much faster and uses less bandwidth than lossless; it is best used when you want speedy data transfer and when the data can lose some of its original makeup.

![Lossless vs lossy compression](https://gisgeography.com/wp-content/uploads/2015/09/Lossy-vs-Lossless-334x425.png)

**Metadata** - Metadata provides more information about other data to make the process easier as a whole. Includes information about files like author, file type, date of creation, etc.

![Metadata](https://static.wixstatic.com/media/21a510_d68674efd9d940e78485d7359045f509~mv2.jpg/v1/fill/w_1000,h_618,al_c,q_90,usm_0.66_1.00_0.01/21a510_d68674efd9d940e78485d7359045f509~mv2.jpg)

**Computer Networking** - Communication between computers; includes internet and direct data transfer. Routing redundancy is important in networking in order to ensure that one computer failure doesn't take down the whole network. Relates to parallel/distributed computing in the sense that computers must communicate and collaborate to accomplish tasks.

![Computer Networking](https://www.guru99.com/images/1/090719_0446_BasicsofCom1.png)

**Parallel vs. Distributed Computing** - Parallel computing is where multiple computers are given different tasks to perform because the tasks are more efficient to run when spread out. Distributed computing is where multiple computers are given the same task to perform in order to speed up its completion.

![Parallel vs distributed computing](https://www.oreilly.com/library/view/distributed-computing-in/9781787126992/assets/e1153739-f551-4f1f-a44a-8effcd193099.png)

**Protocol** - Instructions for computers when trying to communicate. Allows different devices to communicate. Examples would be TCP and IP. 

![Protocol](https://cdn.kastatic.org/ka-perseus-images/6a0cd3a5b7e709c2f637c959ba98705ad21e4e3c.svg)

**TCP/IP** - TCP stands for Transmission Control Protocol and is used in the transfer of data online. IP stands for Internet Protocol and is used to designate addresses to systems which connect to the internet. Both TCP and IP work in tandem to ensure online data transfer runs smoothly.

![TCP/IP](https://www.dnsstuff.com/wp-content/uploads/2020/07/four-layers-TCP-IP.png)

**HTTP** - Hypertext Transfer Protocol(HTTP) is the protocol that allows for the users to interact with other web browsers by transferring data between clients and servers.

![HTTP](https://www.ionos.com/digitalguide/fileadmin/DigitalGuide/Screenshots_2020/diagram-of-http-communication-process.png)

**GET** - The GET method requests and receives data from a web server. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/app.py#L120-L125)

**POST** - The POST method requests that a web server accept the entity enclosed in the request message. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/app.py#L133-L142)

**API/Library** - Application Programming Interface (API) is a procedure of functions in a library, or the place you store the functions, so you can call on them in other parts of your code. [Link to creation of API](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/api/webapi.py) and [link to usage](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/app.py#L120-L125)

**Dependencies** - When a program requires another program to run/work. In python, dependencies are added into files using the "from" and "import" keywords. Dependencies pull from a library of functions and classes to allow programmers to use those classes/functions. Dependencies can be considered a form of abstraction, as you are reusing code into your own project.

![Dependencies](https://www.prince2.com/blog/wp-content/uploads/2019/05/xproject-dependencies-flowcharts.jpg.pagespeed.ic.NhIr7uedka.jpg)

**Import** - Imports files from another program to use in another program. EX Flask, used here: [link to usage](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/app.py#L0-L15)

**MVC** - Model, view, and control. MVC is a way to organize a project; the model of a project includes databases and any backend/algorithmic processes, the view is the frontend and is what is displayed to the user, and the control connects the model to the view, allowing the frontend to access and interact with the backend. [Model folder](https://github.com/tonyhieu/csp-anthonys-harem/tree/main/model), [view (templates) folder](https://github.com/tonyhieu/csp-anthonys-harem/tree/main/templates), and [control file](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/app.py)

**Crud** - Create, read, update, and delete; used for database access. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/db.py#L25-L59)

**Fetch** - Receives data using a program. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/app.py#L43)

**Async** - Events independent of the main program. They interact but don't rely on each other to run. 

![Async](https://www.baeldung.com/wp-content/uploads/sites/4/2020/07/sync.png)

**REST** - Representational state transfer, a standard for APIs to follow. RESTful APIs transfer data in a standardized way, typically JSON files, and allow for verification through headers. [Link to RESTful API](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/api/webapi.py)

**Object Oriented Programming (OOP)** - Object-oriented programming, uses data and code that rely on classes and objects.

![OOP](https://raw.githubusercontent.com/ArjitS1/Raw/master/Student.jpg)

**Class** - Class is the definition of a set of properties which provides the initial values for the code's behavior. [Creation of a database class](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/db.py#L14)

**Attributes** - A property of an object, essentially a variable that is specific to an object. For example, the font-size of an element. [Attributes of objects inside of a database](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/db.py#L15-L18)

**Methods** - A function that is given to an object, typically used to alter attributes inside of the object. [Code that shows CRUD methods for the database objects](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/db.py#L25-L59)

**Object** - A data structure that can be given methods and attributes, main way of handling data in OOP. Classes and objects can usually be used interchangeably to describe the same thing.

![Object](https://javatutorial.net/wp-content/uploads/2014/11/class-object-featured-image.png)

**Procedures/Functions** - Code that preforms tasks and usually returns a value after completing its task, repeats whenever called. [Link to example](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/templates/about.html#L73-L85)

**Sort** - A sort is an algorithm which sorts a list using a distinguishing factor. This could be alphabetical order, greatest to lowest, or something else. [Link to example of selection sort](https://github.com/Altoid0/FRQ-Site/blob/master/src/main/java/com/application/frq/Anthony/Sorts.java#L22-L38)

**Search-Linear/Binary** - A linear search searches through a list to find a single part of that list. A binary search searches through a list to match your searched component by repeatedly halving the list until the location is narrowed down. Binary search runs in O(log(n)) time while linear search runs in O(n) time, meaning that binary search runs faster (consider the end behavior of log n vs. n).

![Search-Linear/Binary](https://s3-us-west-2.amazonaws.com/ib-assessment-tests/problem_images/binary_search.gif)

**Blueprints** - A set of files in a Flask application that contains a mini Flask app within it. A blueprint typically consists of a folder with its own template and app.py files, and it can be "registered" in the main Flask file in order to add it to the website. Blueprints are used for organization of pages. [Link to app.py blueprint file](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/anthony/anthony.py)
