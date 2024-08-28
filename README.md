# SwapShop | Python, Django

SwapShop is a comprehensive online marketplace where users can post items they want to sell and browse items posted by others. This platform is designed to cater to a wide audience, providing a robust and user-friendly environment for buying and selling second-hand items.

## Features

### 1. **User Registration and Authentication**

- **Sign Up**: New users can easily register by providing a username, email, and password.
- **Login & Logout**: Registered users can log in with their credentials and log out from the admin site.

### 2. **Item Posting**
- Users can post items for sale by providing the following details:
  - **Category**: Predefined categories [Toy, Furniture, Clothes].
  - **Name**: User-defined name for the item.
  - **Description**: Detailed description of the item.
  - **Price**: Set by the user.
  - **Picture**: Users can upload an image, with a default blank if not provided.

### 3. **Browsing and Searching**
- Users can browse items using the search function, which matches items based on their name or description.
- **Category Filter**: Users can filter items based on predefined categories.

### 4. **User Communication**
- Each item has a "Contact Seller" button, allowing potential buyers to message the seller directly.
- **Inbox**: Users have an inbox where they can manage conversations, with all previous messages saved for future reference.

### 5. **User Dashboard**
- Users can manage their posted items through their dashboard, with options to:
  - Change the item's name, description, and price.
  - Mark items as sold using the **IS_SOLD** checkbox, which hides the item from the marketplace.

### 6. **Admin Panel**
- Super users (admins) can manage the entire platform, including user accounts, posted items, and user communications, through the Django admin interface.
- **Admin Registration and Access**:
  - To manage the website and access its database, create a superuser (admin) account by running:
    ```bash
    python manage.py createsuperuser
    ```
  - Follow the prompts to create the superuser, typically using "admin" as the username.

# Project Environment Setup

## Setting virtual environment
Open a new Terminal by clicking NewTerminal button on top of you VSCode Terminal section 

Then type in: 
#### python3 -m venv env

Here "env" is the name of your virtual environment
env is an isolated virtual environment just for this project where you can install python packages such as Django 
Upon creating a new virual environment you should be able to see a new folder called env

## Activate virutal environment 
In the same terminal type in:
#### source env/bin/activate 
You should be able to see an (env)/ at the beginning of your terminal directory on your terminal 

## Install django and pillow 
In the same terminal type in:
#### pip install django

After finishing django package then type in:
#### pip install pillow 

## Finish 
When finishing installing these two packages your virtual environment is now ready to run this website! 

# Run the website 
Open a new terminal, and make sure your new terminal path is in the same directory as OnlinMarketPlace-django
If your are not sure, right click on the (OnlineMarketPlace-django) folder beneath (env) folder, and select "Open in Integrated Terminal"
Then you should be on track, and type in: 
#### python manage.py runserver 

You should be able to see the following messages: 

#### System check identified no issues (0 silenced) <br />
#### Django version 4.2.5, using settings 'myproject.settings' <br />
#### Starting development server at http://127.0.0.1:8000/ <br />
#### Quit the server with CONTROL-C. <br />
 
Copy the server address  http://127.0.0.1:8000/ and paste it into your system browser <br />
You should be able to see the fron page of the server with Sign up and Login on top right 

### Login as admin 
On the website you can login with your super user credentials, however it will just perform as a normal user <br />
In order to access admin site, on the url of your brower type in: 
#### http://127.0.0.1:8000/admin 
Login here with your super user credentials and you should be able to access the database of the website <br />
In here you can manage the website users, their items and the conversations between users.

Enjoy!

