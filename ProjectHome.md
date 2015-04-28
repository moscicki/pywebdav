
```
ATTENTION: A security issue in PyWebDAV when being used with 
MySQL (other usecases are NOT affected) has been found. 
This is fixed in version 0.9.4.1 released Feb 18th 2011. 
Please update your installations!
```

## About ##

Python WebDAV implementation (level 1 and 2) that features a library that enables you
to integrate WebDAV server capabilities to your application.

A fully working example on how to use the library is included. You can find a server in the DAVServer package. This server is fully functional and can even be run as daemon.

If you search an easy to use WebDAV server that supports most clients (cadaver, Mac OS X Finder, Windows Explorer, ...) then try out PyWebDAV.

## Usecases ##

  * Calendar Server for iCal (tested on Mac OS X Tiger and Leopard)
  * Simple fileserver
  * Making your application support WebDAV

## Installation ##

Installation and setup of server can be as easy as follows:

```
$ easy_install PyWebDAV 
$ davserver -D /tmp -n -J
Starting up PyWebDAV server (version 0.9.2-dev)
>> ATTENTION: Authentication disabled!
>> Serving data from /tmp
>> Listening on localhost (8008)
```

If you're living on the bleeding edge then check out the sourcecode from
_http://pywebdav.googlecode.com/svn/trunk/_

```
$ svn co http://pywebdav.googlecode.com/svn/trunk/ pywebdav
$ cd pywebdav
$ python setup.py develop
$ davserver --help
```

Send patches to http://code.google.com/p/pywebdav/issues/list

If you want to use the library then have a look at the DAVServer package that
holds all code for a full blown server. Also doc/ARCHITECURE has information for you.


## Questions? ##

Ask here http://groups.google.com/group/pywebdav
or send an email to the maintainer.


## Requirements ##

  1. Python 2.4  or higher (www.python.org)


## License ##

GNU Library General Public License v2 or later


## Contributors ##

```
Cédric Krier
Jesus Cea
Martin Wendt
```

## Author(s) ##

```
Simon Pamies (also current maintainer)
Bielefeld, Germany
s.pamies at banality.de

Christian Scholz
Aachen, Germany
mrtopf at webdav.de

Vince Spicer
Ontario, Canada
vince at vince.ca
```

## Additional notes ##

If you want MySQL based authentication then you need to install the following package and also configure the server using a configuration file.

MySQLdb (http://sourceforge.net/projects/mysql-python)

Look inside the file doc/TODO for things which needs to be done and will be done
in the near future. Have a look at doc/ARCHITECTURE to understand what's going on under the hood