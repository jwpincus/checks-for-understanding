## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What is Webpack and why is it useful?
+ It is a tool that compiles your assets together for production. It minimizes the size and number of assets that a client will require
2. When do you want to use event delegation?
+ When you want to listen for events on child nodes that may not exist at the time that the handler is initialized
3. What's one difference between ES5 and ES6?
+ constructor syntax
4. How are you using the MVC design pattern in your Quantified Self project?
+ the database connection is handled through model files. The controller handles routing, and also generating views from the models
5. How do you execute raw SQL in node?
+ using knex.raw()
6. What's a callback function and what are some reasons when we use/need callback functions?
+ Callback function is a function that fires off after the completion of another function. Use it by passing a function in as the argument to another function
7. What is CORS?
+ it is a javascript rule that prevents making calls to servers different than the origin.
8. What are some steps to avoid CORS?
+ YOu have to explicitly allow cross origin requests in AJAX, and possibly on the server side as well depending on framework.

#### Review  

9. Why do people say "HTTP is stateless"?
+ Every request is made in isolation/without memory from previous requests.
10. What is a RESTful API?
+ an API the serves data based on the route and parameters submitted
11. What are some main characteristics of a team following an agile workflow?
+ Working in parralel on issues. Breaking the work down into granular stories
12. What are some advantages/disadvantages to using OAuth to authenticate a user?
+ Pro: you can authenticate and quickly gather information about a user from a different service. Con: You are relying on another service to be up, and not change in order to keep things going.
