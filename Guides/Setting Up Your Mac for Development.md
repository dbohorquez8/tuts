# Setting Up Your Mac for Development

1. Setup your iCloud account (if any)
1. Install Chrome and Firefox
1. Install Dropbox
1. Download and Install Command Line Developer Tools from the App Store. Alternatively, run ```xcode-select --install```
1. Install Brew http://brew.sh/
1. Install Git ```brew install git```
1. Install zsh ```brew install zsh```
1. Install Postgres ```brew install postgres```
1. Install Imagemagick ```brew install imagemagick```
1. Install curl ```brew install curl```
1. Add your SSH keys for Github https://help.github.com/articles/generating-ssh-keys
1. Install Heroku Toolbelt https://toolbelt.heroku.com/osx
1. Install ohmyzsh https://github.com/miguelperez/ohmyzsh-confs/blob/master/README.md
1. Install Sublime Text
  1. Install Sublime command line
      
      ```ln -s /Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl /usr/local/bin/sublime```

  1. Install Package Control https://sublime.wbond.net/installation
    1. Install packages for highlighting HAML, SASS, Coffeescript, etc.

1. Install RVM http://rvm.io/rvm/install
  1. Install Ruby Versions

    For version 2.1
    ```rvm install 2.1 --with-gcc=clang```

  1. Create a ~/.gemrc file and add these lines:
    
    ```gem: --no-ri --no-rdoc```
