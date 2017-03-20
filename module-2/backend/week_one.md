## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
Get, Post, Put, Delete ....?
2. What is Sinatra?
A framework for serving dynamic websites
4. What is MVC?
Model, View, controller. Three parts to web apps
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
Sinatra recognizes some conventions, and it makes it much easier for others to look into code and change or fix issues
6. What types of variables are accessible in our view templates without explicitly passing them?
Instance variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  @count = 1
  get '/horses' do
    erb :index, :locals{:name => 'Mr. Ed"}
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
9. What's the purpose of ERB?
It lets us build HTML with ruby code embedded in it
10. Why do I need a development AND test database?
Using a development database with testing could lead to unpredictable results in both environments
11. What's responsive design?
HTML/CSS that adapts to a wide variety of screens and devices
12. What is CRUD and why is it important?
Create, Read, Update, Delete. It describes the major actions that you can do with data points in a database
13. What does HTTP stand for? 
Hyper Text Transfer Protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
<% This code runs %> <%= this code renders the return into the html %>
15. What's an ORM?
Object relational model. It describes how different parts of the code interact with the database
16. What's the most commonly used ORM in ruby (Sinatra & Rails)?
ActiveRecord
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
get /restaurants - shows all restaurants
get /restaurants/restaurant shows an individual restaurant
get /restaurant/new shows a view to create a restaurant record
post /restaurant/new sends the new restaurant params into the model and database
get restaurants/restaurant/edit shows a view to edit a restaurant record
put /restaurants/restaurant/edit updates a restaurant record
delete /restaurants/restaurant removes a restaurant record
18. What's a migration? 
A set of instructions for modifying or creating a table in a database
19. When you create a migration, does it automatically modify your database?
No, you have to run a make file 
20. How does a model relate to a database?
A model will interact with a table/s to CRUD records
21. What's the difference between agile workflow and waterfall method?
Agile attacks many granular problems all at once. Waterfall attacks big problems in order
22. What is the difference between `#new` and `#create`?
new creates a record without saving it, create does the same, but also saves it to the db
