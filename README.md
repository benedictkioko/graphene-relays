## Graphene Relays

Relay is a Javascript framework built by Facebook with the purpose of improving the GraphQL architecture by making some core assumptions:

```bash
- A mechanism for refetching an object.
- A description of how to page through connections.
- Structure around mutations to make them predictable.
```

Git clone the project to your machine
```bash
# get the project
git clone https://github.com/benedictkioko/graphene-relays.git
cd graphene-relays/cookbook
```
Next
```bash
# Create a virtualenv in which we can install the dependencies
virtualenv env
source env/bin/activate
```
Install our dependencies:

```bash
pip install -r requirements.txt
```

Now setup our database:

```bash
# Setup the database
./manage.py makemigrations
./manage.py migrate

# Load some example data
./manage.py loaddata ingredients.json

# Create an admin
./manage.py createsuperuser
```
Now you should be ready to start the server:

```bash
./manage.py runserver 0.0.0.0:8000
```

Now head on over to:
[http://localhost:8000/app.api](http://localhost:8000/app.api)
