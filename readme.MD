Solitude is an open source Kafka-GUI, based on Django and React. Solitude is just a practice project, developed for educational and practice purposes. Solitude is not suggested, and was not intended to be used in production environment, with mission critic data.

- Cluster and brokers are defined in Django admin
- Creating topics and increasing partitions will require an admin user

<h1>Django Runs as Backend</h1>
Django runs in backend, you'll need to follow installation steps:

After clonning the repository:
We suggest you to create a virtual environment

<h6>Install Requirements</h6>
Install reqiurements:
<code>pip install -r requirements.txt</code>

<h6>Create Superuser</h6>
Create a super user: You need to create first super user, which will be able to access admin panel. 
<code>python3 manage.py createsuperuser</code>

<h6>Run Server</h6>
Run server: When you run server, admin and api will be up, if migrations are ready.
<code>python3 manage.py runserver</code>

<h6>Allowed Hosts</h6>
Allowed hosts setting defines how many ways you can run React to access Api. Add or remove hosts depending how you want to run React:
<code>ALLOWED_HOSTS = ['0.0.0.0', 'localhost']</code>

<h6>Application Secret Key</h6>
Copy paste .env.local as .env. You will need to add a new secret has to your application. 
<code>python3 -c 'import secrets; print(secrets.token_hex(100))'</code>
Get the output string and add it to your .env file. 


<h1>React Runs as Frontend </h1>
React will need to install all dependancies:
<code>npm install</code>

After the installation, you can run the server with npm start:
<code>npm start<code>

