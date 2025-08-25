# README

First app
In this project, I created a web application for managing personalized movie watch lists. The system allows users to create new lists, view all their lists, and explore the details of each list. Users can bookmark movies into specific lists, leave comments on those bookmarks, and remove bookmarks when they no longer want them. Each list enforces unique names, while bookmarks ensure unique [movie, list] pairings with a minimum comment length. Movies are pre-seeded from the TMDB API, giving users a real collection to build from. The application is fully responsive and styled with Bootstrap, providing a clean and user-friendly interface.

Key Features:

• Create, view, and manage personalized movie lists

•	Add movies to lists with bookmarks + user comments

•	Delete bookmarks and lists (with dependent cleanup)

•	Many-to-many relationship between movies and lists through bookmarks

•	Validations for unique names, unique [movie, list] pairs, and minimum comment length

•	Seeded with real movies (TMDB API proxy)

•	Responsive front-end styled with Bootstrap 5 + custom CSS

<img width="1920" height="958" alt="Screenshot 2025-08-25 at 11 18 46 AM" src="https://github.com/user-attachments/assets/b8f69855-f59b-433d-b423-de2c5701819f" />

<img width="1920" height="958" alt="Screenshot 2025-08-25 at 11 19 35 AM" src="https://github.com/user-attachments/assets/8597a8c5-5616-4c20-9308-a0d3debfac89" />

<img width="1920" height="958" alt="Screenshot 2025-08-25 at 11 40 42 AM" src="https://github.com/user-attachments/assets/f732714c-e176-49ad-8ec1-d278a6b99b9a" />


## Rails app generation

```
rails new rails-watch-list -d postgresql --skip-action-mailbox -T
cd rails-watch-list
```
We then need to create the postgresql database for this new rails app.
```
rails db:create
```
Create a repo on GitHub and push our skeleton.
```
git add .
git commit -m "rails new"
gh repo create --public --source=.
git push origin master
```

Gems used
```
# Gemfile
gem "bootstrap", "~> 5.3"
gem "autoprefixer-rails"
gem "font-awesome-sass", "~> 6.1"
gem "simple_form"
gem "sassc-rails"
```
