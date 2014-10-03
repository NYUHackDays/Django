# Setup

## Pre-requisites
* `Python 2.6` or higher - Higher version is better but 2.6 will do. You're on your own with Python 3.xx version.
   * For **Windows** users, see the last section
* `pip`:
   * Most `*nix` distributions come with `easy_install`. To check if its installed, do `which easy_install`. It should list the path to the file.
   * If the above works, then run this at command line `easy_install pip`. [might require you to install as `admin`]
* `django`: At command line run `pip install django==1.4`
   * To install it manually, especially for **Windows** users, see the last section.
* Bring `Full on Nerdness`


## World is a better place with these
* `Sublime` - You will thank me later. Download [link](http://www.sublimetext.com/)
* `iTerm2` -  Native terminal sucks. Download [link](http://www.iterm2.com/#/section/home)

## Agenda

### Intro

  * Http protocols
  * Webservers & Zombies
  * MVC, MVT, MVP and other crazy acronyms
  * Convention over Configuration

### Django

  * Project Structure
  * Django lightweight webserver - For testing
  * `settings.py`- The bootstrapper
  * Concept of Apps
  * Models
    * Managers
    * Abstract
    * Relationships. Its tough!
  * Views/URLs
    * Class vs Function
    * Decorators -> Don't know, go read python
  * Forms
  * Templates
    * Built in tags/filters
    * Custom tags/filters
  * Admin
  * Django Ecosystem => third party apps 
  * Testing -> Its like eating veggies. Its healthy but sucks.
 
### Be wary of Magic

  * Querying
    * Watch SQL queries in debugger
    * Index as needed
    * South
  * `It works on my machine` execuses
    * Use same database engine
    * Remove hardcoded paths
  * Packaging Conflicts
    * `virtualenv`

### Making it faster
  * Cache, Cache & Cache. Repeat with me
    * Redis, Memcached
  * Only pull what you need
  * Jinja2 Templating

### Further Reading
  * Signals
  * Unit Test
  * Packaging/Deployment
  * Admin
  * Full Django [book](http://www.djangobook.com/en/2.0/index.html)

### Q/A

# Appendix
## For Windows users

### Python
* Install the latest python by going to this [link](http://www.python.org/download/). Install the `2.7` version.
* Install `pip` via this [link](https://sites.google.com/site/pydatalog/python/pip-for-windows).

### Django

* Download the 1.4.x release from [download page](https://www.djangoproject.com/download/1.4.8/tarball/).
* Untar the downloaded file (e.g. `tar xzvf Django-X.Y.tar.gz`, where X.Y is the version number of the latest release). 
* If youâ€™re using Windows, you can download the command-line tool **bsdtar** to do this, or you can use a GUI-based tool such as 7-zip.
* Change into the directory created in step 2 (e.g. cd Django-X.Y).
* If youâ€™re using Linux, Mac OS X or some other flavor of Unix, enter the command `sudo python setup.py install` at the shell prompt. 
* If youâ€™re using Windows, start a command shell with administrator privileges and run the command below. This will install Django in your Python installationâ€™s site-packages directory.

```

      python setup.py install

```


*You should really move to a *nix distro or install [virtual box](https://www.virtualbox.org/wiki/Downloads) and instal *nix on it. You get all these issues with paths, case sensitivity and many more when you run a app developed in windows on linux*
