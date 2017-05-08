# latest-repo
🐍 Flask app, that shows lately updated GitHub repository of Allegro 

## Getting started

These instructions will get you a copy of the project up and running on your local machine

### Prerequisites

In terminal, enter latest-repo folder

Create virtual environment (in example below name will be ‘env’):

```
virtualenv env
```

Enter to your virtual env and type in terminal (note the dot):

```
. bin/activate
```

Cd outside the env and into latest_repo folder, where is requirements.txt and install it:

```
pip3 install -r requirements.txt
```

If you would like to increase API’s raising limit from 60/h to 5000/h, register OAuth application on GitHub to get your client_id and client_secret. Follow instructions from link below:

[GitHub OAuth](https://github.com/settings/applications/new) - Register a new OAuth application

If you created an app, set your environment variables locally. Type in terminal (note that, there are no apostrophes):

```
export client_id=type_your_client_id_here
```

then:

```
export client_secret=type_your_client_secret_here
```

Now open python and type:
```
>>> import os
>>> client_id=os.environ[„client_id”]
>>> client_secret=os.environ[„client_secret”]
```


SOME_SECRET_KEY = os.environ["SOME_SECRET_KEY"]


To check if variables exported properly, enter python in terminal and type:

```
>>> import os
>>> print(client_id)
here will appear your client_id
>>> print(client_secret)
here will appear your client_secret
```
Exit() python


### Run 

When in virtualenv, cd into local-repo folder and type in terminal:

```
python3 latest_repo.py
```

You will see the information:

```
Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

Open your browser. In our app, route is set to: /repo so in address window paste:

```
http://127.0.0.1:5000/repo
```

Voilà! You should see something like picture below, but with current information 🙂

![PrintScreen](https://cloud.githubusercontent.com/assets/22544944/25808798/6955172a-340b-11e7-883f-0fd1442f5240.png)

## Built With

* [Flask](http://flask.pocoo.org/docs/0.12/) - Web framework
* [Flask-Bootstrap](https://pythonhosted.org/Flask-Bootstrap/) - Not too much content, but wanted to see the difference and play a little 😉
* [GitHub API v3](https://developer.github.com/v3/) - Official GitHub API v3
* [PyGitHub](http://pygithub.readthedocs.io/en/latest/) - Library to use GitHub API v3

## Author

* **Marta Żaryn** - *Initial work* - [GitHub](https://github.com/martazaryn), [Twitter](https://twitter.com/martazaryn)
