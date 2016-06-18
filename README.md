# oAuth2Python on Mac
# if not installed brew
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# install pyenv (for changing python version)
$ brew install pyenv

# install python 3.5.1
$ pyenv install 3.5.1

# if error when you install python 3.5.1
$ xcode-select --install

# check pyton versions
$ pyenv versions
  * system
  3.5.1
$ pyenv local 3.5.1
  system
  * 3.5.1
# check pip 
$ pip list

# if not install pip
$ brew install -v python-pip

# install python virtual environment
$ pip install virtualenv
$ mkdir Projects
$ cd Projects
# clone oAuth2Pyton from url
...
# create pyton virtual environment
$ cd Projects
$ virtualenv oAuth2Python_venv
$ ls
   oAuth2Python		oAuth2Python_venv
$ source oAuth2Python_venv/bin/activate
(oAuth2Python_venv) 192-168-1-112: jefflee$ cd oAuth2Python
# run server
(oAuth2Python_venv) 192-168-1-112:oAuth2Python jefflee$ python manage.py runserver

You can see http://localhost:8000
