# django-channel-websocket-server
This is a basic setup and function WebSocket server using channels who is a package that helps us integrate two ways communication features to our Django project. 
Channels build upon the native ASGI support in Django. Whilst Django still handles traditional HTTP, Channels gives us the choice to handle other connections 
in either a synchronous or asynchronous style through Daphne.

For now, we just created a simple chat app that allows us to enter a chat room and start discussing. To make it run on your local machine just follow these few steps:

To get started make sure:
***You have Python3.10.4 running on your local machine; #To check: -Windows user: python --version -Linux/Mac user: python3 --version (install python: https://www.python.org/downloads/)

***Make sure to have Docker installed (We will use docker to run Redis)
***Anny text editor of your choice
*** Make sure you have virtualenv installed on the local machine if not just run this command: pip install virtualenv


Let Go:
First of all clone the repose, open your terminal or console or konsole:
	git clone https://github.com/nelsonmandeladev/django-channel-websocket-server-.git # you can clone it anywhere on your computer (just make sure the current user can rwx on it and you can also rename it)

Next, let's make sure that Redis is ready:
	docker run -p 6379:6379 -d redis:5 #This command will pull a new Redis image if not found in local

Next:
	cd django-channel-websocket-server- or cd <folder_name> if you renamed it
	python -m venv <virtualenv_name> #(windows user)
	python3 -m venv <virtualenv_name> #(linux/mac user)

You will see a new folder <virtualenv_name> in your project root
Now let's activate our virtual virtualenv
	source <virtualenv_name>\Script\activate #(windows user)
	source <virtualenv_name>\bin\activate #(Linux/mac user)
	
Next, we will install all needed packages of our project
	pip install -r requirements.txt

Next, we can make some migrations using this command:
	python manage.py migrate #(Windows, Linux and mac user)

Once everything is migrated let's run our dev server:
	python manage.py runserver
	
Now let's see if our chat app is working correctly by opening this URL in any browser:
	 http://127.0.0.1:8000/
	 Click on Let simply chat button
 	 In the input, bar enter a room name "eg: hello" and heat enter
	 Open a new tab or a different browser and do the thing
	 
	 Enjoy !!!!! You have a simple chat room running on your computer
	
For any questions, just open an issue here or contact me:
	discord: nelsonmandeladev
	email: sonfacknelsonmandela@gmail.com
	git: https://github.com/nelsonmandeladev

More feature like: Session authentication, users in room listing and online status, allow your custom world, who is typing, message read status and run live on heroku

Question: For this exemple i didn't allow users to type their own message, guest why ? :)
	
	
	
	
	
