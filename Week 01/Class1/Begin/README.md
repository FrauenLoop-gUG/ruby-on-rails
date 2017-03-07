## Hello World!

This is our introduction to Ruby on Rails. At the end of this lesson, we'll have a webpage (think website) 
running on <http://localhost:3000> with the words "Hello World!"  

- Open an application called "Terminal"
- Go to folder where you want to create the project
- run `rails new HelloWorld`
  You'll see a whole lot of output on the screen, pretty cool right! Wait till the printing stops
- run `cd HelloWorld`
  You're now in a "rails project"
- run `bundle install`
  More output on the screen, again, wait till it stops
- run `rails server`
  This time there will be a lot less output
- Finally open <http://localhost:3000> in you favorite browser
  You should see a really pretty website
- Go back to the Terminal and hit `Ctrl+C`
- run `rails generate controller Welcome index`
  A little more output will show up on the screen
- Now open the app/views/welcome/index.html.erb file in your _text editor_.  
Delete all of the existing code in the file, and replace it with the following single line of code:  
  `<h1>Hello, Rails!</h1>`
- Now open the file config/routes.rb in your editor.
- Just below the line `get 'welcome/index'` add this line `root 'welcome#index'`
- Make sure both files are saved and then go back to the Terminal
- run `rails server` one more time
- Finally open <http://localhost:3000> in you favorite browser ... Tada!!!

