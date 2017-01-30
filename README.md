# Ruby on Rails Tutorial: sample application

**This repository is out of date and is no longer maintained. Please see the [Rails Tutorial Help page](http://railstutorial.org/help) for the most up-to-date version.**


This is the sample application for
[*Ruby on Rails Tutorial: Learn Web Development with Rails*](http://railstutorial.org/). You can use this reference implementation to help track down errors if you end up having trouble with code in the tutorial. In particular, as a first debugging check I suggest getting the test suite to pass on your local machine:

    $ cd /tmp
    $ git clone git@github.com:oleksandrbyk/olek-rails3-sample.git
    $ cd olek-rails3-sample
    $ cp config/database.yml.example config/database.yml
    $ bundle install
    $ bundle exec rake db:migrate
    $ bundle exec rake db:test:prepare
    $ bundle exec rspec spec/

If the tests don't pass, it means there may be something wrong with your system. If they do pass, then you can debug your code by comparing it with the reference implementation.