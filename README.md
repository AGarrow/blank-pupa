## Dependencies

[Uninstall MacPorts](http://guide.macports.org/chunked/installing.macports.uninstalling.html) and [uninstall Fink](http://www.finkproject.org/faq/usage-fink.php#removing) if you are using either. Then, [install Homebrew](http://mxcl.github.io/homebrew/#selectable) if you haven't already.

Ensure Homebrew is up-to-date and ready to brew:

    brew update
    brew doctor

Use Homebrew's Python:

    brew install python

Install Git:

    brew install git

Install MongoDB and follow the post-installation instructions:

    brew install mongodb

You can refer to the instructions at any time with:

    brew info mongodb

### Virtualenv

Install virtualenv and virtualenvwrapper:

    sudo pip install virtualenv virtualenvwrapper
    mkdir $HOME/.virtualenvs

Find out what shell you are using:

    echo $SHELL

If you are using bash, run:

    echo "export WORKON_HOME=\$HOME/.virtualenvs" >> $HOME/.bashrc
    echo "source /usr/local/bin/virtualenvwrapper.sh" >> $HOME/.bashrc
    source $HOME/.bashrc

If you are using zsh, run:

    echo "export WORKON_HOME=\$HOME/.virtualenvs" >> $HOME/.zshrc
    echo "source /usr/local/bin/virtualenvwrapper.sh" >> $HOME/.zshrc
    source $HOME/.zshrc

## Getting Started

In the `mkvirtualenv` command below, replace `pupa` with your project's name:

    mkvirtualenv pupa
    git clone git://github.com/opennorth/blank-pupa.git
    cd blank-pupa
    pip install -r requirements.txt

## Troubleshooting

If you want to work on your project again later, remember to first load the virtual environment:

    workon PROJECT_NAME

## Bugs? Questions?

This repository is on GitHub: [http://github.com/opennorth/blank-pupa](http://github.com/opennorth/blank-pupa), where your contributions, forks, bug reports, feature requests, and feedback are greatly welcomed.

Copyright (c) 2013 Open North Inc., released under the MIT license
