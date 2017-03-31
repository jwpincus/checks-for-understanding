## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?
+ $ rails new
2. What do Models generally inherit from in rails?
+ ActiveRecord::Base
3. What do Controllers generally inherit from in a rails project?
+ ActionController
4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
+ resources :horses, only: [:show]
5. What rake task is useful when looking at routes, and what information does it give you?
+ rake routes gives you alisting of the path prefix, verb, URI, and method associated with each route
6. What is an example of a route helper? When would you use them?
+ Route helpers are ways of internally telling rails where you are referring to using the route prefix and necessary arguments
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
+ `_url` will return the full path with domain name(?), `_path` will return just the local path
8. What are strong params and why are the necessary?
+ strong params control what can be passed into your controller in the params. They require you to explicitly allow the keys that you want to prevent a user from reassigning protected values.
9. What role does `form_for` play in helping us create our forms?
+ it 'automagically' sets up methods and routes based on the object that is given in the argument
10. How does `form_for` know where to submit the user's input?
+ it makes assumptions based on the object passed in, or a route can be explicitly assigned
11. Create a form using a `form_for` helper to create a new `Horse`. 
```ruby
<%= form_for Horse.new do |f| %>
<%= f.text_field :name %>
<%= r.submit "Make me a horse" %>
<% end %>
```
12. Why do we want to validate our models?
+ to make sure that we don't duplicate records, or to make sure that all necesarry data is included
