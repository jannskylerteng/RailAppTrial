# README

# RailAppTrial

Create Rails App (postgresql as database)
- rails new blog -d postgresql

Start postgre
- brew services start postgresql

Create the database
- rails db:migrate:reset
- rails db:seed
- bin/setup

- rails db:create

Generate new controller
- rails generate controller Welcome index

Set root page
- config/routes.rb
- add "root 'welcome#index'"

Creating new resource
- config/routes.rb
- add "resources :articles"
- run "rails routes"

Generate controller for articles
- run "rails generate controller Articles"

Create action in Articles controller
- controllers/articles_controller.rb
- add "def new
       end"

Create new template for new action of Articles controller
- create "new.html.erb" in views/articles

Create forms using form builder and the helper method form_with

Create action "create" in Articles controller
- run "rails generate model Article title:string text:text"

Migrate db
- run "rails db:migrate"



