# latest-repo
🐍 Flask app, that shows lately updated GitHub repository of Allegro 

## Getting started

These instructions will get you a copy of the project up and running on your local machine. 

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

Cd outside the env, where is requirements.txt and install them:

```
pip3 install -r requirements.txt
```

If you would like to increase API’s raising limit from 60/h to 5000/h, register OAuth application on GitHub to get your client_id and secret_id. Follow instructions from link below:

[GitHub OAuth](https://github.com/settings/applications/new) - Register a new OAuth application

If you created an app, set your environment variables locally. Type in terminal (Note that, there are no apostrophes):

```
export client_id=type_your_client_id_here
```

then:

```
export client_secret=type_your_client_secret_here
```

To check if variables exported properly, enter python and type:

```
>>> import os
>>> os.environ[‘client_id’]
here will appear your client_id
>>> os.environ[‘client_secret’]
here will appear your client_secret
```

### Installing

When in virtualenv, cd into local-repo folder and type in terminal:

```
python3 latest-repo.py
```

You will see information:

```
Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

Open your browser. In our app route is set to /repo so in address window paste:

```
http://127.0.0.1:5000/repo
```

Voilà! You should see something like picture below, but with current information 🙂

![PrintScreen](https://cloud.githubusercontent.com/assets/22544944/25808798/6955172a-340b-11e7-883f-0fd1442f5240.png)