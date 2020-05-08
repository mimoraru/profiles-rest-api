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