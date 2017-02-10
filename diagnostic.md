# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The purpose of the backend is to store and retrieve data that is generated while a user is using an application. The backend allows a better UX as the user can potentially save progress of their current session and save data to later come back to it. The backend also allows for user authorization and authentication so not just anyone can store and retrieve data on the server.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The Model
```

Which layer in the MVC pattern communicates with the model?

```md
The Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Because we are using a serializer in lieu of our views
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
The Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Read: Index/Show
Create: Create
Update: Update
Delete: Destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. When a client makes a GET request to a particular URL the web server will receive the data and pass the URL and request type (verb) to the router.
2. The router then interprets the data and matches it to a controller action in the controller.
3. The controller action will send a request to the model which tells it to grab the information of the first id of the people table.
4.  The model sends this information back to the controller when sends the information the view which ultimately is what is displayed on the client's browser.
5.  The data that is transfered to the view by the controller includes HTML, CSS, XML, JavaScript, and JSON.
6.  Finally the response is sent to the server and finally back to the user in the form of a HTTP response.
```

What is the command to generate a new rails-api app?

```bash
bin/rails generate new
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
- bin/rails db:drop
- bin/rails db:create
- bin/rails db:setup
- bin/rails db:migrate
- bin/rails db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:string age:integer
```
