## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?
+ Getting a good understanding of JS syntax. Probably could have frontloaded (optionally?) some of the work from this week into the intermission
2. What are some tools to help debug JavaScript code?
+ Debugger for client side
+ Pry for node/server side
+ Head scratchingly bad error messages
3. What are some tools you need in order to unit test your JavaScript?
+ Node Mocha Chai. 
+ A far better understanding of asynchronous JS. 
4. What is the syntax for invoking a function?
+ define with `function funcName(args){ do the things when called;}; funcName`
+ unnamed define and call with `function(args){ the things to do right now;}`
5. What's the difference between `==` and `===` in JavaScript?
+ == will do type conversions automatically so ` 4 == '4' == true ` => true, === is strict with types
6. What's the difference between asynchronous and synchronous JavaScript? 
+ Synchronous will act like ruby and execute in the order it is called. Async uses black magic to do things at the same time, and ruin the intention of your code
7. How do we setup a route when creating an API with Node and Express?
``` var app = express()
app.get('/your-route-here', function(){
the things to return
})
```
8. What do we use Knex for?
+ Knex is an ORM/database connection tool. Its like if you asked me to write my own version of ActiveRecord, that is it doesn't do a lot that you would expect it to.
9. What's `npm` and what do we use it for?
+ it manages and installs dependent packages

#### Review  
10. What's the MVC design pattern? Describe each part of MVC?
+ Model: the layer for processing, managing and manipulating data
+ View: The layer for formatting data for presentation to the outside user
+ Controller: The layer that controlls the flow of a request/response to call the correct views and models 
11. What is AJAX? What are some benefits of using AJAX?
+ Asynchronous JS And XML. AJAX lets you fetch/push data after a page or view has already been loaded client-side. This lets you send and receive information over HTTP without reloading the entire page.
12. What's a background worker? When would we want to use a background worker?
+ Background workers are a way of queuing time intensive jobs that don't need to be completed immediately (image processing, email sending, etc). Use them for things that aren't required for a succesful response. You can also use them for scheduled tasks (sending reminder emails, updating caches, clearing unneeded data)
