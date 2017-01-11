# README

```
gem install rails
rails new blog
cd blog
rails server     (start rails server)
rails generate controller Welcome index (create a controller called Welcome w/ an action (view) called index)
(modify index.html.erb => whatever you want)
(add root 'welcome#index' to config/route.rb; creates index route)
(add resources :articles to config/route.rb; creates RESTful routes for /articles)
rails routes     (view routes)
rails generate controller Articles     (creates the controller for articles)
(add the new method to the articles controller)
(create a new file at app/views/articles/new.html.erb, and add form content using a form builder, provided by the helper method form_for)
(add the create method to the articles controller)
rails generate model Article title:string text:text     (creates an Article model)
rails db:migrate     (runs the db migration)
(update the create method in the Article controller to initialize the Rails model and save it in the database, and redirect the user)
(add the show method in the Article controller)
(create an html template at app/views/articles/show.html.erb)
(add an index method in the Articles controller)
(create an html template for the articles index, at app/views/articles/index.html.erb)
(add links to all the pages)
(add validation to the Articles model)
(modify the Articles controller to handle data validation)
(modify new.html.erb to handle errors)
(create an edit method in the Articles controller)
(create an edit.html.erb file in app/views/articles/)
(create an update method in the Articles controller)
(add links to edit articles in the articles index page and page for each article)
(create a partial for form template _form.html.erb in app/views/articles/)
(modify the new and edit templates to use the form partial)
(add destroy method to Articles controller)
(add a destroy link for articles on the index page)
```