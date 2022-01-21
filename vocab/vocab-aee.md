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

**Lossless vs. lossy compression** - Lossless compression reduces all loss of data and is best used when you want to preserve the original data. Lossy compression loses some data but is much faster and uses less bandwidth than lossless; it is best used when you want speedy data transfer and when the data can lose some of its original makeup.

**HTTP** - Hypertext Transfer Protocol(HTTP) is the protocol which allows for the users to interact with other web browsers by transferring data between clients and servers.

**Computer Networking** - Communication between computers; includes internet and direct data transfer. Routing redundancy is important in networking in order to ensure that one computer failure doesn't take down the whole network.

**Parallel vs. Distributed Computing** - Parallel computing is where multiple computers are given different tasks to perform because the tasks are more efficient to run when spread out. Distributed computing is where multiple computers are given the same task to perform in order to speed up its completion.

**Protocol** - Instructions to do when something happens.

**TCP/IP** - TCP stands for Transmission Control Protocol and is used in the transfer of data online. IP stands for Internet Protocol and is used to designate addresses to systems which connect to the internet. Both TCP and IP work in tandem to ensure online data transfer runs smoothly.

**GET** - The GET method requests and receives data from a web server. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/app.py#L120-L125)

**POST** - The POST method requests that a web server accept the entity enclosed in the request message. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/app.py#L133-L142)

**MVC** - Model, view, and control. MVC is a way to organize a project; the model of a project includes databases and any backend/algorithmic processes, the view is the frontend and is what is displayed to the user, and the control connects the model to the view, allowing the frontend to access and interact with the backend. [Model folder](https://github.com/tonyhieu/csp-anthonys-harem/tree/main/model), [view (templates) folder](https://github.com/tonyhieu/csp-anthonys-harem/tree/main/templates), and [control file](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/app.py)

**Crud** - Create, read, update, and delete; used for database access. [Link to code](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/db.py#L25-L59)

**Fetch** - Receives data using a program.

**Async** - Anything that happens in the background of loading that doesn't require user input. Typically used to get data from an API at a different time than the load time of the website. Used with await functions, involves a promise from the receiver to the sender

**REST** - Representational state transfer, a standard for APIs to follow. RESTful APIs transfer data in a standardized way, typically JSON files, and allow for verification through headers. [Link to RESTful API](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/api/webapi.py)

**API/Library** - Application Programming Interface (API) is a procedure of functions in a library, or the place you store the functions, so you can call on them in other parts of your code. [Link to creation of API](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/api/webapi.py) and [link to usage](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/app.py#L120-L125)

**Object Oriented Programming (OOP)** - Object-oriented programming, uses data and code that rely on classes and objects.

**Class** - Class is the definition of a set of properties which provides the initial values for the code's behavior. [Creation of a database class](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/db.py#L14)

**Attributes** - A property of an object, essentially a variable that is specific to an object. For example, the font-size of an element. [Attributes of objects inside of a database](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/db.py#L15-L18)

**Methods** - A function that is given to an object, typically used to alter attributes inside of the object. [Code that shows CRUD methods for the database objects](https://github.com/tonyhieu/csp-anthonys-harem/blob/026649638b3ff997fbbbbfad13ba515be4506192/db.py#L25-L59)

**Object** - A data structure that can be given methods and attributes, main way of handling data in OOP. Classes and objects can usually be used interchangeably to describe the same thing.

**Procedures/Functions** - Code that preforms tasks, repeats whenever called.

**Data/Procedural Abstraction** - Data abstraction is where you separate the logistics of the data from how it is represented. Procedural abstraction is where you separate the logistics of an action taken from how it is implemented into the code.

**Sort** - A sort is an algorithm which sorts a list using a distinguishing factor. This could be alphabetical order, greatest to lowest, or something else. [Link to example of selection sort](https://github.com/Altoid0/FRQ-Site/blob/master/src/main/java/com/application/frq/Anthony/Sorts.java#L22-L38)

**Search-Linear/Binary** - A linear search searches through a list to find a single part of that list. A binary search searches through a list to match your searched component by repeatedly halving the list until the location is narrowed down.

**Blueprints** - A set of files in a Flask application that contains a mini Flask app within it. A blueprint typically consists of a folder with its own template and app.py files, and it can be "registered" in the main Flask file in order to add it to the website. Blueprints are used for organization of pages. [Link to app.py blueprint file](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/anthony/anthony.py)

**Metadata** - Metadata provides more information about other data to make the process easier as a whole. Includes information about files like author, file type, date of creation, etc.