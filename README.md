##Relay
Relay is a Javascript framework built by Facebook with the purpose of improving the GraphQL architecture by making some core assumptions:

```bash
- A mechanism for refetching an object.
- A description of how to page through connections.
- Structure around mutations to make them predictable.
```

```bash
# Get the example project code
git clone https://github.com/graphql-python/graphene-django.git
cd graphene-django/examples/cookbook
```
Next
```bash
# Create a virtualenv in which we can install the dependencies
virtualenv env
source env/bin/activate
```
Now we can install our dependencies:

```bash
pip install -r requirements.txt
```

Now setup our database:

```bash
# Setup the database
./manage.py migrate

# Load some example data
./manage.py loaddata ingredients

# Create an admin user (useful for logging into the admin UI
# at http://127.0.0.1:8000/admin)
./manage.py createsuperuser
```
Now you should be ready to start the server:

```bash
./manage.py runserver 0.0.0.0:8000
```

Now head on over to
[http://localhost:8000/app.api](http://localhost:8000/app.api)