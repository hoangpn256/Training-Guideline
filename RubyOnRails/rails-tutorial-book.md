## Ruby on Rails Tutorial Book Guideline

* [Chapter 1,2](#chapter1-2)
* [Chapter 3, 4, 5](#chapter3-4-5)
* [Chapter 6](#chapter6)
* [Chapter 7](#chapter7)
* [Chapter 8](#chapter8)
* [Chapter 9](#chapter9)
* [Chapter 10](#chapter10)
* [Chapter 11](#chapter11)
* [Chapter 12](#chapter12)
* [Chapter 13](#chapter13)
* [Chapter 14](#chapter14)

***

<a name='chapter1-2' />

### Chapter 1, 2
* Chapter 1 - From zero to deploy
* Chapter 2 - A toy app

#### Objective

* Get a high-level overview of Ruby on Rails programing and web development in general

* Understand about a Rails project structure

* Know some kind of command in Ruby on Rails

#### Outline

* About Ruby on Rails
> An open source web-application framework written by Ruby

> Available under the generous MIT License

>Fully digest and implement the REST architectural style

* Create new app

* Project Structute

* MVC Model

* RESTful

* Macro

#### Conclusion

* Capture the basic elements of Ruby on Rails framework and how they interact
with each other

* Know how to use basic commands in Ruby on Rails

#### Exercises

* Create new app with specific version 5.1.2

* Using migration scaffold to generate User with some attributes name, age, phone, emails

* Add attributes date_of_birth and gender into User model without drop your database.

* Show user with new information (date_of_birth and gender)

* Write out the analogous steps for visiting the URL /users/1/edit

***

<a name='chapter3-4-5' />

### Chapter 3, 4, 5
* Chapter 3 - Mostly static pages
* Chapter 4 - Rails-flavored Ruby
* Chapter 5 - Filling in the layout
#### Objective

* Begin developing the sample application, this will be completed in our course.

* The most solid foundation in Rails-flavored Ruby.

* Start filling in the custom stylesheet by incorporating a CSS framework

#### Outline

* Static pages

* Slightly dynamic pages

* Rails layout

* Navigation pages

* Bootstrap and custom css

#### Conclusion

* See basic how to rails plays.

* Overview of Ruby language.

* How to Bootstrap can be used in rails application.

#### Exercises

* Make a Contact page for the sample app with for the title “Contact | Ruby on
Rails Tutorial Sample App”.

* What should you do if you want after visiting the website, you see hello your name and see title “Contact | Ruby on Rails Tutorial Sample App”?

* Create controller micropost and when you visit your website, you can see all
micropost

***

<a name='chapter6' />

### Chapter 6 - Modeling users

#### Objective

* Active Record & Active Record LifeCycle

* Generation

* Secure Password

#### Outline

* Mockup
* Model
    * Generate

    * Functions with model

    * Validation & Callback

* Secure Password

#### Conclusion

* How to validate the user's birthday must be in the last 100 years?

* Where is method **has_secure_password?** Which this method will be
provided by? How does this method work?

#### Exercises

* How to validate the user's birthday must be in the last 100 years?

* Where is method "has_secure_password"? Which this method will be
provided by? How does this method work?

#### References

* [Ruby on Rails Guide - Active Record Validation](https://guides.rubyonrails.org/active_record_validations.html)

* [Ruby on Rails Guide - Active Record Query](https://guides.rubyonrails.org/active_record_querying.html)

***

<a name='chapter7' />

### Chapter 7 - Sign up

#### Objective

* Create new user in our application

* Using HTML form to sign up user

* Implement REST architecture for user

#### Outline

* Show user

* Signup form

* Unsuccessful signups

* Successful signups

#### Conclusion

* The form_for helper is used to generate forms for interacting with Active Record objects.

* Signup failure renders the new user page and displays error messages automatically determined by Active Record.

* Rails provides the flash as a standard way to display emporary messages.

* Signup success creates a user in the database and redirects to the user show page, and displays a welcome message.

#### Exercises

* Display the created_at and updated_at attributes to the user show page

* When you sign up, you must fill in your birthday and gender. Birthday input is
where you can choose date and gender you can choose between three
values: female, male, other

***

<a name='chapter8' />

### Chapter 8 - Basic login

#### Objective

* Our sample application has a fully functional login and authentication system.

* Basic knowledge about sessions

#### Outline

* Sessions

* Create login form

* Authenticate

* Login

* Logout

#### Conclusion

* Rails can maintain state from one page to the next using temporary cookies via the session method.

* The login form is designed to create a new session to log a user in.

* The flash.now method is used for flash messages on rendered pages.

* Using the session method, we can securely place a user id on the browser to create a temporary session.

* We can change features such as links on the layouts based on login status.

#### Exercises

* What is the difference between GET login_path and POST login_path?

* Log in with a valid user and inspect your browser’s cookies. What is the value of the session content? Hint: If you don’t know how to view your browser’s cookies, Google for it

***

<a name='chapter9' />

### Chapter 9 - Advanced login

#### Objective

* Use permanent cookies to implement **remember me** function so user can still login to the site even browsers closed.

* Add ability to optionally remember users using **remember me** checkbox

#### Outline

* Remember token and digest
* Login with remembering
* Forgetting users
* **Remember me** checkbox

#### Conclusion

* Transformed application into a site with full functions of signup and login behaviors

* Complete the authentication functionality, restrict access to pages based on

login status and user identity
* Learn to use persistent cookies via the cookies method

* Associate to each user a remember_token and a corresponding remember_digest for persistent sessions

* Sign users out by deleting user's session id and remove permanent cookie from browser

#### Exercises

* By finding the cookie in your local browser, verify that a remember token and encrypted user id are present after logging in

* After logging out, verify that the corresponding cookies have been removed from your browser.

***

<a name='chapter10' />

### Chapter 10 - Updating, showing, and deleting users

#### Objective

* Complete the REST actions for the Users resource by adding edit, update, index, and destroy actions

* Build a simple user profile and updating

* Make a listing of all users with pagination

* Allow administrative users delete other users, wiping them clear from the database

#### Outline

* Update user

* Show list users

* Delete users

#### Conclusion

* Users can sign up, log in, logout, view their profiles, edit their settings, and see an index of all users—and some can even destroy other users.

* The sample application forms a solid foundation for any website requiring users with authentication and authorization

#### Exercises

* Create Laptop model has two attributes: title and content with validation: max
length of title is 250 characters

***

<a name='chapter11' />

### Chapter 11 - Account activation

#### Objective

* Implement an account activation step to verify that user controls the email they used to sign up

* Associating an activation token and digest with a user

* Sending user an email with a link including the token

* Activating the user upon clicking the link

#### Outline

* Account activations resources

* Account activation emails

* Activate the account

* Email in production

#### Conclusion

* Our sample application’s sign up, log in and log out machinery is nearly complete.

* Next chapter will be allowing users to reset their passwords when they forget.

* Account activation can be modeled as a resource despite not being ActiveRecord objects.

* Rails can generate Action Mailer actions and views to send mail, supports both plain-text and HTML mail.

* Account activations use a generated token to create unique URL for activation

#### Exercises

* Send mail to user after first login

* Deploy your code and using Gmail mail server to send email

***

<a name='chapter12' />

### Chapter 12 - Password reset

#### Objective

* Use a resource that is not a Active Record object

* Understanding the basics of Action Mailer.

* Use token to ensure safety request

* It is possible to configure and use mail on the product environment

#### Outline

* Mockup UI

* Password reset resource

* Password reset email

* Reset password

#### Conclusion

* Like sessions and account activations, password resets can be modeled as a resource despite not being **Active Record** objects.

* Rails can generate **Action Mailer** actions and views to send email (supports
both plain-text and HTML mail).

* Environment variable.

#### Exercises

* After clicking on the link we will be directed to the page with the correct password reset ?

* After reset password, send user's password through email with content:
**You just changed your password, sign in again so we know it's you! Click here**
Click this underline statement, you will go to login page

***

<a name='chapter13' />

### Chapter 13 - User microposts

#### Objective

* Add a new resources microposts - short messages posted by a specific user.

* Learn about new relationship has_many and belongs_to ombination.

* Make form and partials needed to manipulate and display microposts.

* Users can create and delete their own microposts with image.

* Users can see other user microposts.

#### Outline

* Mockup

* Micropost Model

* Micropost View

* Micropost Controller

* Micropost Images

* Other note

#### Conclusion

* We can model a user having many microposts using the has_many and belongs_to methods in the User and Micropost models, respectively.

* The has_many/belongs_to combination gives rise to methods that work through the association.

* The code user.microposts.build(...) returns a new Micropost object automatically associated with the given user.

* Scopes take anonymous functions as arguments.

* Options of association (like **dependent: :destroy**)

* It is possible to pass variables to Rails partials.

* Microposts, like Users, are modeled as a resource backed by an Active Record model.

#### Exercises

* Modify user's profile page **app/views/users/show.html.erb**, so that you can
**write a micropost** when **accessing** this page

***

<a name='chapter14' />

### Chapter 14 - Following users

#### Objective

* Add a social layer that allows users to follow (and unfollow) other users.

* Resulting in each user’s Home page displaying a status feed of the followed users’ microposts

* Understand about through association in Rails

* Basic knowledge about Rails ajax

#### Outline

* Relationship model

* Stats and follow form

* Following and followers pages

* The status feed

#### Conclusion

* Using new kind of Rails association: **has_many :through**

* Using Rails ajax to render follow button and update number **follower / following**

* New way to register a routes

#### Exercises

* In a show user screen, display all micropost by that user and the followers

* In a user’s profile, display all people this user follow

* Using jquery ajax to make follow and unfollow instead of rails ajax