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

If you would like to register OAuth application on GitHub

[GitHub OAuth](https://github.com/settings/applications/new) - Register a new OAuth application



Register new OAuth application on GitHub to get client_id and secret_id: https://github.com/settings/applications/new


Set your environment variables locally:
export SOME_SECRET_KEY=1c3-cr3am-15-yummy

To access environment variables from one of your settings files:
import os
SOME_SECRET_KEY = os.environ["SOME_SECRET_KEY"]



http://stackoverflow.com/questions/14786072/keep-secret-keys-out-with-environment-variables

