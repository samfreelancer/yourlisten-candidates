## Personal details

Name: Sameer Arora

Country: India 

Hourly Rate: $15/hr

Timezone: GMT +5:30

Skype Id: samfreelancer

## Availability

Are you able to work from 3PM to 7PM (GMT -2) ? In case you aren't, what's your availability?
Yes, I usually work at night. From 8:00 PM to 03:00 AM which is 12:30 PM to 07:30 PM. I hope this will work.
 
## Tech Skills

Assing yourself a score in the following technologies:


Object Oriented Programming (OOP) - 4/5

Git -  4/5

PHP 5 - 4/5

CakePHP framework - 4/5

MySQL -  3.5/5

Javascript - 4/5

jQuery -  3.5/5

HTML - 4/5

CSS - 4/5

## Questions About OOP:

- How do you declare a function or method that you want to be accessed without instantiate the class?

Define menthod as static. It will be accessed by syntax classname::menthodname.

- How do you create a child class of BaseClass ?

extend the child class from parent class.

class A extends B{}
 
## Questions about GIT:

- If you accidentally add the wrong files to be commited using git add, how do you unstage them?
use the reset command if want to keep changes of last of commit. 
git reset --soft HEAD^
This will move the head to the previous commit and keep the changes done as it is. Now we can see the changes by status command.

- If you want to switch to another branch, what command you need to execute?
git checkout branchname: this command will switch between branches.
 
## Questions about PHP 5:

- Please write a conditional block of code that check if the variable $var exists, is not null and it's a number.
if(isset($var) && !is_null($var) && is_numeric($var)){}

- Write a function that adds a line to a log file the current date and time with this format: "[2013-09-23 00:3 0:15] - Status OK"
function markDateTime(){

 $status = "Status OK";
 $content = date('[Y-m-d H:i s:II frac]').' - '.$status;
 $file=fopen("log file path","a");
 fwrite($f,$content,strlen($content)); 
 fclose($file);
 
}

## Questions about CakePHP

- Which is the default path where you set up the configuration for the database?

app/Config/database.php

- How you can get the value of a session variable with key "foo" using CakePHP ?
$this->Session->read('foo');

## Questions about MySQL

- Write a single query to retrieve the information from 2 tables that are related( users and users_data) where the primary key on users is ID and the foreign key on users_data is USER_ID.
SELECT us.*, usd.* FROM users as us, users_data as usd WHERE us.ID = usd.USER_ID;

- Write a single query to retrieve all the queries that are currently running on the server .
show processlist;

## Questions about Javascript

- How do access to the alt attribute of the following image element using javascript? <img src='http://example.com/image.jpg' id='some_img' alt='lol' />
document.getElementById('some_img').getAttribute('alt');

- What is the protocol name behind ajax?
XMLHttpRequest

## Questions about jQuery

- Write a piece of javascript code using jQuery that make the el ement with id "someElement" to appear on the screen using a fade in effect after the DOM is loaded.
$(document).ready(function(){
 $('#someElement').fadeIn();
})
- How do you remove an element from the DOM using jQuery?
 $('#element_id').remove();

## Questions about HTML

- Which is the doctype syntax for HTML5?
<!DOCTYPE html> 

- Which is the attribute and value required on forms to allow file uploads?
enctype="multipart/form-data"
## Questions about CSS

- Which is the css property and its value to force to hide the scroll on any DOM element with fixed height when its content exceed its own height?
overflow:hidden;

- If you have to div elements next to each other with the property float:left, which CSS property do you need to add to the next element in order to get both of them to fill the same height on page and make the next one not a floating one?
float:right;

## Questions about Linux / Unix based OS

- Which protocol(s) you could use to connect to a server SHELL remotely?
ssh

- Write a command to look for the word "ads" on all files with .ctp extension in the same directory
- grep -r 'ads' *.ctp
