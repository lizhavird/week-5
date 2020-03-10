# ASSESSMENT 5: Interview Practice Questions

Answer the following questions. First, without external resources. Challenge yourself to answer from memory. Then, research the question to expand on your answer. Even if you feel you have answered the question completely on your own there is always something more to learn.   

1. Rails follows an MVC pattern. What does that mean?

  Your answer:
multi
v
controller 
??
  Researched answer:
model
view
controller

meaning first, a browser sends a request, which is received by a web server and passed on to the rails router. the router receives the request and redirects to the appropriate controller class method based on the routing URL pattern.
then the controller takes over to render info from the model on the browser. 

2. What is a gem?

  Your answer:
  shiny

  Researched answer:
gem is a code library which is accessable to all. 


3. Why is it important to have validations in your application?

  Your answer:
  
if you do not have validations in your applications, forms will submit without required information, websites could crash due to confusion//lack of data to process. 

  Researched answer:

"Data validation is vital to ensure the data is clean, correct and useful."

4. Describe a possible relationship between a model called Person and a model called Computer. Based on your description, which model would hold the foreign key?

  Your answer:
both would hold a foreign key. 
  Researched answer:
  
a foreign key can only hold the values which are present in the primary key. 
null values are not allowed in the primary key, but they are allowed in the foreign key. 
therefore, person would be the primary key & computer would be the foreign key, as computer would probably not hold values different that person.

5. What is object-relational mapping?

  Your answer:
mapping in relation to an object
  Researched answer:
object relational mapping is a method for storing, retrieving, updating, and deleting from an object oriented program in a database.  

## Looking Ahead: Terms for Next Week

Research and define the following terms to the best of your ability.
- RESTful routes
a way to pull and push data based on user input
- json
javascript object notation, a data representation format
- API
- application programming interface, usually uses json. 
an api is a way to transmit data. it takes requests and tells a system what to do, then returns in the info back to you. 
- Endpoints
i found multiple definitions, im not sure if you are talking about endpoint in api, or endpoint device, ect. 
- Strong params
strong parameters is a feature of rails that prevents assigning request parameters to objects unless they have been explicitly permitted