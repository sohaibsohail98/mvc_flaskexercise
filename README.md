#Model View Controller - MVC:
#View - Web browser

from flask import Flask

#import flask
```python
#in order for us to use flask we need to create a instance of our app

app = Flask(__name__)

```

#Syntax to create flask instance

#syntax for decorators to create a web route

```python
#block of code for default page
@app.route("/")

#define what page the information will be displayed


#Create a welcome method to display on home/default page
def index():
    return "<h1>Welcome to MVC with flask project</h1>"
#end of block of code for default page
```
```@app.route("/<username>") ```
#exercise - create a function called welcome_user
#create a decorator to link the page /user
#return "welcome to Python flask app dear (user)
```python


def welcome_user(username):

    return f"<h1>Welcome to Python flask app dear {username} </h1>"                                                                   
```


#This is an example of how an argument could be passed through welcome user

#Another exercise:
```python


@app.route("/aboutus")

def aboutus_page():
    return "<h2> Welcome to our about us page, Sohaib Enterprises </h2>"                                                                        
```


#index method will be called at the endpoint
#index method will display on our home page
```python 
#syntax to run our app
if __name__ == "__main__":
    app.run(debug=True)     # this ensures to update any changes without re-running the app.

```
