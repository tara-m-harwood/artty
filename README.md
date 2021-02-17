ArTTY Women
When you think about art, are you missing half the picture?
Explore the work of great women artists through our reccomendations based on your taste or mood!

Table of contents
General info
Intro Video
Technologies
Setup
Features
Status
Inspiration
Contact
License

General info
Since 2016, 

Intro Video
TacoLandia on YouTube

Technologies
Ruby - version 2.6.1
ActiveRecord - version 5.2
Sinatra - version 2.0
Sinatra-activerecord - version 2.0
SQLite3 - version 1.4
Setup
To run this project, install it locally by cloning the GitHub repository and typing:

ruby config/environment.rb
Code Examples
def self.get_taco_details(taco)
    returned_taco = Taco.find_by(name: taco)
    puts "Name: " + returned_taco.name + " Taco"
    puts "Protein: " + returned_taco.protein
    puts "Heat Level: " + returned_taco.heat_level.to_s
    puts "Shell Type: " + returned_taco.shell_type
end
def self.update_user_name(user_name)
    old_name = User.find_by(name: user_name)
    puts "What is your new name friend?"
    user_input = gets.chomp
    old_name.update(name: user_input)
    user_input
end
Features
Browse tacos by protein type
Return a random taco from the database
See taco details
Save tacos to favorites list
Remove tacos from favorites list
Take the Taco Compatibility Quiz
To-do list:

Refactor “code smell”
Add API functionality to return a recipe for chosen taco
Discover local restaurants serving tacos
Integrate matching photos to tacos
Status
Project is: finished with option to expand functionality and DRY out code.

Inspiration
The inspiration for TacoLandia came from a restaurant API that did not return the information we were looking for. Using our own love of tacos, we set out to build a fun, interactive, and clean UX/UI that would bring other users joy!

Contact
Created by Catherine O'Hara and Taylor Stein

Feel free to contact us!!! 🌮

License
Click to view