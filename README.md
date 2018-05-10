# Sinatra
Sinatra is a [DSL](1) stripped down to the minimal, to provide basic routing for HTTP applications.
It is a great tool for developing API`s. It depends on Rake to create the interface behind Sinatra.

## The ```app``` Directory
This directory contains model-view-controller for the application.

### The ```app/controllers```  Directory
Controllers ties other controllers together, it is responsible for interactions and is the interface to the application.

### The ```app/models```  Directory
Models represent a component who is responsible for the behaviour and data of the application.

### The ```app/views```  Directory
Views are views of the application components, the templates are in ERB (embedded Ruby)

## The ```config```  Directory
Config contains your ```environment.rb``` file, connecting files to its ```gems```.

## The ```db```  Directory
DB holds your database schema and migrations.

### The ```db/migrate```  Directory
Use ```rake db::create_migration NAME=create_users```

## The ```public```  Directory
Public holds the assets: css, js, and images.

## The ```spec```  Directory
Spec holds the tests for the application.

## ```config.ru``` File
Rack uses this file to build Rake based applications. (Rake is the Make for Ruby). It loads your application, code, libs, and determines which controller to load.

## ```Gemfile``` File
This file holds the ```gems``` required for the application. Use ```bundle install``` to install the dependencies. Use ```bundle init``` to create it.

## ```Rakefile``` File
Rakefile is where custom application tasks are defined. Use ```rake -T``` to see all tasks.


# Setup
* Initialise the ruby environment ```rbenv local 2.5.0```.
* Install ```bundle``` using ```gem install bundle```
* Initialise ```Gemfile``` using ```bundle init```
* Add sinatra using ```bundle add sinatra```

# Test
Add ```helloworld.rb``` and run ```ruby helloworld.rb```

[1]: Domain specific language