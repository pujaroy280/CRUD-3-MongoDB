# CRUD-3-MongoDB

# About

This project is a simple CRUD (Create, Read, Update, Delete) application that utilizes Node.js, Express, body-parser middleware and MongoDB. This part of the CRUD app demonstrates us leveraging MongoDB to store data and interact with the stored data.

## Technologies
- Node.js
- Express
- Body-parser
- MongoDB and Client
- IDE/Editor: [Visual Studio Code]
- Terminal: [Git Bash]

## Getting Started

The project is designed to guide you through the process of storing data and interacting with the stored data using MongoDB client. Follow the steps below to get started:

### Step 1 - Create your POST endpoint

#### index.html

Although this is called a CRUD app, we are using GET, POST, PUT, and DELETE HTTP requests. As mentioned before, we used the GET request to read our data, which means now we will use a POST request to create our data. We can do this using a `<form>` element.

In the body of your `index.html`, add the following:

```html
<form action="/users" method="POST">
  <input type="text" id="username" placeholder="Username" name="username" />
  <input type="text" id="password" placeholder="Password" name="password" />
  <button type="submit">Submit</button>
</form>
```

**IDE/Editor:** [Visual Studio Code]

**Terminal:** [Git Bash]

### Step 2 - Parse the data

 Parse the data by installing body-parser and including that in the app. 
 App will use body-parser for each HTTP request. We can test the POST request and receive information from the index.html in the req itself via the body.

In your browser, test the input fields by providing FAULTY usernames and passwords. You should receive a message in your console - a JavaScript object with the keys username and password.

![image](https://github.com/pujaroy280/CRUD-2-Create/assets/62675121/159816d5-cb86-41e0-9967-4ec4c113e19b)
![image](https://github.com/pujaroy280/CRUD-2-Create/assets/62675121/e27c404e-3873-47c5-b8eb-c0d2c7d86a53)



## Installation
To install and run the project, follow these steps:
1. Clone the repository: `git clone <repository-url>`
2. Navigate to the project folder: `cd <project-folder>`
3. Install dependencies: `npm install`
4. Run the server: `npm run dev`
