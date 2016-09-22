
# Install Jekyll on Ubuntu 14.04 LTS

Along the process described [here](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#platform-linux).


## Install ruby version 2.0 or greater

Use the `apt-get` packaging system (updating it first):

    sudo apt-get update
    
Installing `software-properties-common` allows installing personal package archives in the next step:   

    sudo apt-get install software-properties-common
    
Add the Brightbox ruby PPA:

    sudo apt-add-repository ppa:brightbox/ruby-ng
    sudo apt-get update
    
Install Ruby 2.3:    
    
    sudo apt-get install ruby2.3
    sudo apt-get install ruby2.3-dev
    
## Install Jekyll    
    
Install Bundler:

    sudo gem install bundler

Create a Gemfile in the local git repository.
Add the following code to a text file called `Gemfile`.

    source 'https://rubygems.org'
    gem 'github-pages', group: :jekyll_plugins
    
Install Jekyll and other dependencies from the GitHub Pages gem:

    sudo bundle install
    
    






    