# Notes

Notes about setting up a RoR blog application from scratch

## Init

```bash
    apt-get install -y ruby sqlite3 libsqlite3-dev
    ruby -v
    sqlite3 -v
    sqlite3 --version
    gem install rails
    rails --version
    rails new blog
    cd blog
    bin/rails server
    bin/rails generate controller Welcome index
    bin/rails generate controller Articles
    bin/rails generate model Article title:string text:text
    bin/rails db:migrate
    bin/rails generate model Comment commenter:string body:text article:references
    bin/rails db:migrate
```

## Resources 

https://guides.rubyonrails.org/getting_started.html
https://weblog.rubyonrails.org/2012/3/21/strong-parameters/