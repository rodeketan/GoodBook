# Library 
It is a book review website where a user can login and search for a book by its title, author name or ISBN number. Users can also see reviews from other users and can write their personal reviews about the book too. Users can also see ratings from popular website 'Goodreads'. The complete website is responsive. An API is also included which returns the JSON object containing details about the book and its ratings.
## Login Page
![alt text](https://github.com/rodeketan/library/blob/main/Images/Screenshot%20(299).png)

## Home Page
![alt text](https://github.com/rodeketan/library/blob/main/Images/Screenshot%20(301).png)

## Search Results
![alt text](https://github.com/rodeketan/library/blob/main/Images/Screenshot%20(302).png)

## Review Page
![alt text](https://github.com/rodeketan/library/blob/main/Images/Screenshot%20(303).png)

## API
![alt text](https://github.com/rodeketan/library/blob/main/Images/Screenshot%20from%202021-06-18%2007-31-37.png)
***

1. **books.csv-** CSV file containing details of books to be exported to Heroku Database.

2. **import.py-** Python file written to insert data from CSV file into the Heroku Database.

3. **helpers.py-** Python file containing definition of the 'login_required()' function.

4. **application.py-** This is the main application file written in Python.

5. **static folder-** This foldder conatins an image file and a CSS file named style.css.

6. **templates folder**

This folder contains 7 HTML files.
  
  1. _**layout.html**_
     
    This is the basic html layout file. It is inherited by other html files.
  2. _**login.html**_

    This file contains the html for the login page.
  3. _** register.html**_
   
    This file contains the html for sign up page.
  4. _**index.html**_

    This file is loaded when an user successfully logs in.
  5. _**results.html**_

    This file contains the html for displaying the results of search.
  6. _**book.html**_

    This file contains the html for displaying the details of a particular book when it is being searched by the user.
  7. _**error.html**_

    File for displaying errors.

### Tables
- books(id, isbn, title, author, year)
- users(id, username, hash)
- reviews(id, user_id, book_id, comment, rating, time)



