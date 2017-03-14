## My Portfolio! - Static Pages

Today we'll add more pages to our Hello World app. In the end we'll have simple "home" & "about" pages.

- Open an application called "Terminal"
- Go to folder where you want to create the project
- run `rails new myPortfolio`
  You'll see a whole lot of output on the screen, pretty cool right! Wait till the printing stops
- run `cd myPortfolio`
  You're now in a "rails project"
- run `bundle install`
  More output on the screen, again, wait till it stops
- run `rails server`
  This time there will be a lot less output
- Finally open <http://localhost:3000> in you favorite browser
  You should see a really pretty website
- Go back to the Terminal and hit `Ctrl+C`
- Open the "myPortfolio" direcory (a.k.a folder) in your favorite "text editor"
- Go to the config/routes.rb file
- Below the line `Rails.application.routes.draw do` add `get 'static_pages/home'`  
  Don't forget to save.
- Now open the app/controllers directory and create a new file called `static_pages_controller.rb`
- Add the following to the file
```
class StaticPagesController < ApplicationController
end
```
- Now open the app/views/ and create the direcotry `static_pages` and inside create a file called `hello.html.erb`  
  Add following single line of code:  
  `<h1>Home</h1>`
- Make sure both files are saved and then go back to the Terminal
- run `rails server` one more time
- Finally open <http://localhost:3000/static_pages/home> in you favorite browser ... Tada!!!
- Think about the steps we went through, could you add an "About" page at <http://localhost:3000/static_pages/about> ?

Notice the file `static_pages_controller.rb` & the dir `static_pages/`
- What do they have in common?
- How are they related to `config/routes.rb`
