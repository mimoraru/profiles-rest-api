# Profile REST API

First trial to create a REST API

1. Create the vagrantfile for the development server: vagrant init ubuntu/bionic64
2. Copy the server config: see the curent vagrantfile in the project
3. Run the vagrant server: vagrant up
    3.1. Connect to the vagrant server: vagrant ssh
    3.2. Go to vagrant file on the server: cd /vagrant
    3.3. Add the python virtual environment: python -m venv ~/env
    3.4. Activate the python virtual environment: ~/env/bin/activate
    3.5. Install the requrements in the virtual environment: pip install -r requirements.txt
    3.6. Create the django project file: django-admin.py startproject profiles_project .


## User API Features Features
### Create new profile
* handle registration of new users
* Validate profile data

### Listing existing profiles
* search for profiles by email or name

### Viewing a specific profile
* using the profile ID

### Updating the profile of the loggend in user
* change name, email and password

### Delete profile

## API URLs
### /api/profile/ 
* list all profiles when the HTTP GET method is called
* create new profile when  HTTP POST method is called

### /api/profiles/<profile_id>
* view specific profile details by using HTTP GET
* update object using HTTP PUT/PATCH
* remove it completely using HTTP DELETE

## Feed API 
### Features
* Create feed items for logged in users
* Update feed items
* Deleting feed items
* viewing other users feed items

### End point: /api/feed/ 
* list all feed items
* GET (list feed items)
* POST (create feed items for logged in users)

### End point: /api/feed/<feed_item_id>
* manage specific feed items
* GET (get the feed item with its details)
* PUT / PATCH (update feed item)
* DELETE (delete feed item)

