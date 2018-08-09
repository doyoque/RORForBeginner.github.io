# Installation

If you prefer the official Documentation please visit [Guides.rubyonrails.org](http://guides.rubyonrails.org).
## Setup And Install

This instruction will lead you to setup and install the environment of ruby programming language and ruby on rails.

### Install dependencies
The first things before we install the ruby programming language, we need to download some dependencies that require for ruby. Run this command at your terminal to download and install the dependencies.
```
$ sudo apt-get update
$ sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
```
### rbenv

Now the dependencies already installed. Next we need to install `rbenv`. This tools is using for version control of ruby installation. Which mean you can install one or more version of ruby in your computers.
```
$ cd ~
$ git clone https://github.com/rbenv/rbenv.git ~/.rbenv
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
$ exec $SHELL
```
### ruby-build

Next install the ruby-build. Because rbenv need the `ruby-build` for build the source of ruby code. 
```
$ git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
$ echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
$ exec $SHELL
```
### ruby
Now we can install the Ruby with `rbenv`. For example we install ruby with 2.4 Version.
```
$ rbenv install 2.4.0
$ rbenv global 2.4.0
$ ruby -v
``` 
### Install Ruby On Rails

After that we install the Ruby On Rails with RubyGems. What is RubyGem? According to [RubyGems](https://en.wikipedia.org/wiki/RubyGems) - RubyGems is a package manager for the Ruby programming language that provides a standard format for distributing Ruby programs and libraries. RubyGems come alongside with Ruby installation. So when you already installed Ruby you will also have the RubyGems. Let's install the Ruby On Rails by running this command.
```
$ gem install rails
``` 
It will download and install the Ruby On Rails. After that check the installation by typing
```
$ rails --version
$ Rails 5.2.0
```
Nice one. Now Ruby and Ruby On Rails are ready on your computer.