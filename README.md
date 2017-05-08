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
pip install -r requirements.txt
```

If you would like to increase API’s raising limit from 60/h to 5000/h, register OAuth application on GitHub to get your client_id and secret_id. Follow instructions from link below:

[GitHub OAuth](https://github.com/settings/applications/new) - Register a new OAuth application

If you created an app, set your environment variables locally. Type in terminal:

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



http://stackoverflow.com/questions/14786072/keep-secret-keys-out-with-environment-variables

