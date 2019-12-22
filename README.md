# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version 6.0.1

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## Adding porfolios items via rails generator
1. Generate a resource for portfolio items then migrate
```sh
$ rails g resource Portfolio title:string subtitle:string body:text main_image:text thumb_image:text
Running via Spring preloader in process 4853
      invoke  active_record
      create    db/migrate/20191222020540_create_portfolios.rb
      create    app/models/portfolio.rb
      invoke  controller
      create    app/controllers/portfolios_controller.rb
      invoke    erb
      create      app/views/portfolios
      invoke    helper
      create      app/helpers/portfolios_helper.rb
      invoke    assets
      invoke      scss
      create        app/assets/stylesheets/portfolios.scss
      invoke  resource_route
       route    resources :portfolios
$ rails db:migrate
== 20191222020540 CreatePortfolios: migrating =================================
-- create_table(:portfolios)
   -> 0.3071s
== 20191222020540 CreatePortfolios: migrated (0.3072s) ========================
```
