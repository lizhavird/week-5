# ASSESSMENT 5: Rails Practical Questions

1. What is the command to create a new Rails application with a Postgres database?

$ rails new dog_app -d postgresql -T
$ cd dog_app
$ rails db:create
$ rails server


2. Explain each section of the following route:  get '/library/:id' => 'book#show'

get - retrieve this file url from the designated folder
library - library is connected in the routes file, which connects all the components to the main controller
:id - id is the variable which you are manipulating to render
book - book is the controller which library is conencted to
show - show is the variable which you are manipulating to render the command - "show"

3. Oops, I forgot to add a foreign key to my model. Describe the steps to remedy this mistake.

first we will need to define the association between the model and class.

ex:

class Person < ApplicationRecord
  has_many :shirts
end

class Shirts < ApplicationRecord
  belongs_to :person
end

then we will need to migrate the updated associations w/ rails db:migrate

then we will need to attatch the shirts owned to a person and save the variable association. 
$ rails c
bob = Person.first
bob.save
bob.shirt.create shirt: "blue"

4. What is the command to generate a Rails model for a person table with columns named shirt, pants, and shoes?

$ rails generate model Person shirt:string pants:string shoes:integer



5. I want to add validations to the model from question 4 to ensure no one can make a new entry without data in all the columns. How do I do that?

class Person < ApplicationRecord
  validates :shirt, :pants, :shoes, presence: true
end