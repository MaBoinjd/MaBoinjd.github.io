---
title: Isaac and Samuel Vocabulary
permalink: /vocab/is
layout: default
---

[Back to vocab page](/vocab)
<br />
[Back to main page](/)

# Vocabulary

1. **Binary/Hexadecimal, Bit, Nibble, Byte**

**Binary/Hexadecimal** - Binary is a base 2 system used by computers to represent data with 1's and 0's. Hexadecimal is a base 16 system that serves a similar purpose. It is often used for representing colors in hex format.
```$bg-color-light: #fff9d4;
$header-color-light: #fff9d4;
$nav-text-color-light: #0e1f33;
$content-text-color-light: #0e1f33;
$top-gradient-color-light: #fff9d4;
$bottom-gradient-color-light: #fbf4b5;
```
![Binary](http://www.sciencefriday.com/wp-content/uploads/2015/08/UTF8-Table-7802.png)

**Bit** - Bits are binary digits, the smallest unit of data in computing. A bit can either be a 1 or a 0, representing on or off.
* ```at_school = True``` The digit is either True (1) or False (0)

**Nibble** - A nibble is 4 bits or half a byte. This can also be represented as one hexadecimal digit.

**Byte** - Bytes are strings of 8 bits each. These are the smallest usable units for computer storage.
![](https://www.researchgate.net/profile/Ozlem-Akinci-Sozer/publication/309168674/figure/fig2/AS:613447184162844@1523268614702/An-example-of-the-kind-of-byte.png)


2. **Data, Data Abstraction**

**Data** - Data is info that's been converted into a binary form for computers.

![](https://media.geeksforgeeks.org/wp-content/uploads/13-1.png)

**Data Abstraction** - Data abstraction is separating what is shown on the outside and the internal data that isn't shown. The user will only see the most important information while hiding the background stuff.

3. **Lossless/Lossy Compression** - Both lossless and lossy compress files, causing lost data. But, lossless compresses less compared to lossy. Lossless is often used for text and images, while lossy is also used for images, but also with videos.

![](https://vivadifferences.com/wp-content/uploads/2021/05/images-1.png)

4. **Metadata** - Metadata is basically data about other data. This data about another piece of data would allow that data to be identified. For example, metadata for an ebook may include the author and the date published. 

![](https://miro.medium.com/max/500/1*y3bST2DnCmDTQzD5YnamTw.png)

5. **Computer Network, Parallel/Distributed computing**

**Computer Network** - A computer network is multiple computers connected to each other while being able to communicate with each other.

**Parallel/Distributed computing** - Parallel computing is when a bunch of smaller computations from a larger computation are being performed at the time. Distributed computing is connecting multiple computers and running these computers together as a single system.

![](https://www.oreilly.com/library/view/distributed-computing-in/9781787126992/assets/e1153739-f551-4f1f-a44a-8effcd193099.png)

6. **Protocol, TCP/IP, HTTP, GET, POST**

**Protocol** - Protocols are rules that determine how multiple devices will communicate with sending and receiving data. This allows different devices to communicate despite possible differences between them.

**TCP/IP** - TCP/IP stands for Transmission Control Protocol/Internet Protocol. This basically allows computers to communicate when they are far away from each other. TCP is used to make sure the info sent is secure. IP allows differentiating and identifying separate computers, devices, systems, etc.

**HTTP** - HTTP stands for "HyperText Transfer Protocol", which is a protocol connecting web browsers and servers, sending things such as HTML pages to the user. 
![](https://miro.medium.com/max/689/1*4SEvcz6KvyaqOqBpJABTBg.png)

**GET** - GET requests have all the data needed in the URL.
```@app.route("/about")
def about():
    anthony_response = requests.request("GET", domain + "/api/anthony")
    isaac_response = requests.request("GET", domain + "/api/isaac")
    ethan_response = requests.request("GET", domain + "/api/ethan")
    erik_response = requests.request("GET", domain + "/api/erik")
    samuel_response = requests.request("GET", domain + "/api/samuel")
    return render_template("about.html", anthony=anthony_response.json(), isaac=isaac_response.json(), ethan=ethan_response.json(), erik=erik_response.json(), samuel=samuel_response.json())
```

**POST** - POST requests give extra data from the browser to the server in the message body. The difference between GET and POST requests are how data is sent to the server.
```@app.route("/login", methods=['POST', 'GET'])
def login():
    if request.method == 'POST':
            username = request.form['username']
            password = request.form['password']
            dbHandler.insertUser(username, password)
            users = dbHandler.retrieveUsers()
            return render_template('index.html', users=users)
    else:
        return render_template('login.html')
```

7. **Library, Dependencies, Import**

**Library** -  Libraries are collections of many things that can be used in coding, such as files, scripts, functions, etc. 

**Dependencies** - A dependency is when a program requires another one to run. So this means a program is basically relying on another for it to work.

**Import** - Import is bringing files from a different program and converting them to a file format that can be used in the program that the user is using.

```import flask```

8. **Web API, REST, FETCH, Async, Request, Response**
**Web API** - API stands for "application programming interface", which allows communication between applications. APIs can be used to pull data from things like libraries. 

```@isaac_bp.route("/")
def isaac_index():

    url = "https://na1.api.riotgames.com/lol/platform/v3/champion-rotations"

    headers = {
                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.93 Safari/537.36",
                "Accept-Language": "en-US,en;q=0.9",
                "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                "Origin": "https://developer.riotgames.com",
                "X-Riot-Token": "RGAPI-3b547dc9-429a-4977-9258-252aad4c3d5a"
            }

    response = requests.request("GET", url, headers=headers)

    print(response.text)
    output = json.loads(response.text)
    return render_template("isaacIndex.html", lol=output)
```

**REST** - REST is an architectural style for making standards between computers, allowing easier communication.

**FETCH** - FETCH is for getting data from somewhere to be used in the user's program.

**Async** - Async programming is a type of parallel programming that allows a program to run outside of the main program/process.

**Request** - Requests are used for computers to communicate with each other, with one computer sending a request and the one receiving the request responding to it.

**Response** - Response is done in the second part of a request-response method, responding to the request sent by another computer.

9. **Blueprints** - Blueprints can be used to organize a Flask application. A blueprint has a group of templates, static templates, and py files. This allows large applications to be a lot more simplified and organized together. 

![](https://uploads.gravitatedesign.com/legacy/blueprint_for_coding.jpg)

10. **MVC** - MVC stands for "Model-View-Controller", which is often used for user interfaces and data. This is made to separate the display and the data, which would allow one to change without changing the other. The model focuses on data logic, the view focuses on bringing the info from the model to the user, and the controller changes the view when data changes.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a0/MVC-Process.svg/640px-MVC-Process.svg.png)

11. **Code Sequence, Procedures/Functions, Procedural Abstraction**

**Code Sequence** - Code sequence is performing a function with certain commands in a certain order. This allows functions with multiple steps to run correctly. 

**Procedures/Functions** - Procedures are parts of code that do a certain function. They are essentially instructions for the computer to do whatever the program was meant to do. Functions are similar to procedures but are used to return outputs from certain inputs.
```@app.route("/update/<id>", methods=["GET", "POST"])
def update(id):
    game = Games.query.filter_by(gameID=id).first()
    if request.method != "POST":
        return render_template("update_database.html", game=game, id=id)

    new_title = game.title
    new_author = game.author
    new_embed = game.embed

    if request.form["title"] is not None:
        new_title = request.form["title"]
    if request.form["author"] is not None:
        new_author = request.form["author"]
    if request.form["embed"] is not None:
        new_embed = request.form["embed"]

    try:
        game.update(title=new_title, author=new_author, embed=new_embed)
    except:
        return render_template("404.html", error_message="Something went wrong with updating your game.")

    return redirect("/games_database")
```

**Procedural Abstraction** - This entails heavily simplifying what is shown compared to what is really going on behind the scenes. For example, this would be like running a program and using it without understanding or needing to understand the code being used or using variable parameters to do something.
![](https://miro.medium.com/max/728/1*IdZcSRFX9EkccyBPz09gmA.jpeg)

12. **OOP, Class, Attribute, Method, Object**

**OOP** - This stands for "Object-Oriented Programming", which means that it revolves around objects instead of functions. These objects can contain data and/or code.  

**Class** - A class is used to make one or more objects that are used in object-oriented programming. This allows objects to have specific variables or parameters instead of the whole program using them.

**Attribute** - This is a portion of the code that can be set to different values making it change some characteristics and components of the program whether it be its look, or how the program runs.
![](https://user.oc-static.com/upload/2018/12/19/15452208786759_Capture%20d%E2%80%99e%CC%81cran%202018-12-19%20a%CC%80%2013.01.02.png)

**Method** - Methods are similar to functions, but can only be called by an object. Methods allow objects to do specific functions.
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR-b1qbagXJYNRIjoJRbeUN7V9UEnyVUnenajLQhtmnmBRx-dnqCfMxearjWOndwpgpuNI&usqp=CAU)

**Object** - Objects are things that represent something and are referenced, which contain certain values. These can be variables, variables, or data structures.
```
isaac_bp = Blueprint('isaac', __name__,
                       url_prefix='/isaac',
                       template_folder='templates',
```

13. **CRUD** - CRUD stands for create, read, update, delete. CRUD is used for things that store information, such as databases.
![](https://s33046.pcdn.co/wp-content/uploads/2018/12/word-image-228.png)

14. **Sort, Search-Linear/Binary**
**Sort** - Sort is an operation that puts items into an order. With this, items are first inputted, then operations happen to sort these items, and finally, the sorted list is outputted. 

```
list = [10,2,7,3,5]
sorted(list)
```
output = [2, 3, 5, 7, 10]

**Search-Linear/Binary** - A linear search goes through a list/array in order before finding the specified item. Binary search finds an item in a list/array by splitting the list that may have the item into 2 over and over again until only one possible item is left.

