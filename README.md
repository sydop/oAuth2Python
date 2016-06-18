## oAuth2Python on Mac
#### if not installed brew
<pre>
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
</pre>
#### install pyenv (for changing python version)
<pre>
$ brew install pyenv
</pre>
#### install python 3.5.1
<pre>
$ pyenv install 3.5.1
</pre>
#### if error when you install python 3.5.1
<pre>
$ xcode-select --install
</pre>
#### check pyton versions
<pre>
$ pyenv versions
  * system
  3.5.1
$ pyenv local 3.5.1
  system
  * 3.5.1
</pre>
#### check pip 
<pre>
$ pip list
</pre>
#### if not install pip
<pre>
$ brew install -v python-pip
</pre>
#### install python virtual environment
<pre>
$ pip install virtualenv
$ mkdir Projects
$ cd Projects
</pre>
#### clone oAuth2Pyton from url
<pre>...</pre>
#### create pyton virtual environment
<pre>
$ cd Projects
$ virtualenv oAuth2Python_venv
$ ls
   oAuth2Python		oAuth2Python_venv
$ source oAuth2Python_venv/bin/activate
(oAuth2Python_venv) 192-168-1-112: jefflee$ cd oAuth2Python
</pre>
#### run server
<pre>
(oAuth2Python_venv) 192-168-1-112:oAuth2Python jefflee$ python manage.py runserver
</pre>

#### connect to sqlite (default database)
<pre>
(oAuth2Python_venv) 192-168-1-112:oAuth2Python jefflee$ python manage.py dbshell
SQLite version 3.8.10.2 2015-05-20 18:17:19
Enter ".help" for usage hints.
sqlite> 
</pre>

###You can see http://localhost:8000
