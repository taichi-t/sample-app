# Ruby on Rails turorial to build an rails application
  
This is a repository for an application built with the following materials
[*Ruby on Rails turorial*](https://railstutorial.jp/)
[Michael Hartl](http://www.michaelhartl.com/) 

## LICENCE

[Ruby on Rails turorial] More details, please see (https://railstutorial.jp/)
The code is published under MIT Licence and Beerware.
More details, please see [LICENSE.md](LICENSE.md)

## Usage
First, clone the repository to your local environment, and then execute the following command to install Gems.

```
$ bundle install --without production
```

After that, migrate db.

```
$ rails db:migrate
```

Finally, make sure that it works well by executing tests.

```
$ rails test
```

You are ready to build Rails server if tests all are passed.

```
$ rails server
```

More detail, Please see [*Ruby on Rails tutorial*](https://railstutorial.jp/)

## Memo
### revert generated code

ex) Contoroller

```
$ rails generate controller StaticPages home help
$ rails destroy controller StaticPages home help
```

ex) Model

```
$ rails generate model User name:string email:string
$ rails destroy model User // no need params such as name:stirng or email:string
```

ex) DB

```
$ rails db:midrate
$ rails db:rollback // Revert to the last version.
$ rails db:migrate VERSION=0 // Revert to the initial version.
```