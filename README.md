
In this project I made a book review website where a user can login and search for a book by its title, author name or ISBN number. User can also see reviews from other users and can write his personal review about the book too. User can also see ratings from popular website 'Goodreads'. The complete website is responsive. An API is also included which returns the JSON object containing details about the book and its ratings.




1. books.csv
 
This is the main CSV file from where I imported the books data to my Heroku Database.

2. import.py

Python file written to insert data from csv file into the Heroku Database.

3. helpers.py

In this Python file I have defined the 'login_required()' function.

4. application.py
 
This is the main application file written in Python.

5. static folder

This foldder conatins an image file and a CSS file named style.css.

6. templates folder

This folder contains 7 HTML files.
  
  1. layout.html
     
    This is the basic html layout file. It is inherited by other html files.
  2. login.html

    This file contains the html for the login page.
  3. register.html
   
    This file contains the html for sign up page.
  4. index.html

    This file is loaded when an user successfully logs in.
  5. results.html

    This file contains the html for displaying the results of search.
  6. book.html

    This file contains the html for displaying the details of a particular book when it is being searched by the user.
  7. error.html

    File for displaying errors.

I have used three tables.

1. books(id, isbn, title, author, year)
2. users(id, username, hash)
3. reviews(id, user_id, book_id, comment, rating, time)


# ENV Variables
$ export FLASK_APP = application.py # flask run
$ export DATABASE_URL ="postgres://ytgsqitccrontf:63128cc39825c010041506b53808ce2a7455c78fcd28daa59e223b7c23f1fe22@ec2-34-232-147-86.compute-1.amazonaws.com:5432/d2ecll3gabfldb"
$ export GOODREADS_KEY ="V3UTmmnnNhiHYLoSUc2DSg" 

