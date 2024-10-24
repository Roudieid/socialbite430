## Frontend Set Up
1. make sure you are inside the frontend folder:
```
cd frontend
```

2. install the node module packages
```
npm install
```

3. start running the application
```
npm run dev
```

if there are any package not being install, then it will tell you in the terminal or the website application, and just install by entering `npm install <package to install>`


## Step to setup the database in postgresql
1. Download PostgreSQL, and make sure its running. For my case, I have used homebrew to download and start the PostgreSQL

```
brew install psql
brew services start postgresql
```

2. create your account in postgresql to have access through entering
```
createdb <your  username>
```

3. enter the following to connect to the postgresql:
```
psql
```

4. Add the password for the user you created for security
```
ALTER USER <your username> WITH PASSWORD 'your_password';
```


5. Enter the following to set up the database that we will be using for this project
```
CREATE DATABASE social_bite;
```

# Steps to use Visual Studio to see the postgresql database
1. Install PostgreSQL by Chris Kolkman inside visual studio
2. After install, it will show up on your side bar with an icon of visual studio
3. After click onto the icon, add a new database connection by clicking on the + button
4. Hostname: localhost, user: the username you used to create database, password: password you used, port: 5432, standard connection. Finally, choose the database "social_bite" that was created. 

## Step to setup a backend
1. Cd into the backend
```
cd backend
```

2. inside the terminal enter the following to download all the needed package:
```
npm install
```

3. start the backend application by entering the following
```
npm start
```

and if there are any missing package, it will tell you in the terminal and just download it by entering `npm install <package to install>`


After you finish all the steps above, you should see this.
    - currently the login function is working with the account
        "janeDoe@gmail.com" and password of "password"
    - the sign up feature is also working

![alt text](https://file%2B.vscode-resource.vscode-cdn.net/var/folders/rj/tmk97wjn4b32pg1nm4q3br180000gn/T/TemporaryItems/NSIRD_screencaptureui_ZJMFvk/Screenshot%202024-10-24%20at%205.12.40%E2%80%AFPM.png?version%3D1729804366378)