README for book2pad
===================

book2pad is a simple script for transferring books(PDF or EPUB) from linux machine to ipad. Jailbreaking is not needed. Tested working with iOS 8.3, 9.1.

Requirements
------------

* install `ifuse <http://www.libimobiledevice.org>`_ on your computer
* biplist should be installed in case your plist file is compressed. (Just run "sudo easy_install biplist" and type your password.)

Usage
-----

If the iPad's contents don't show up immediately after plugging in, mount your ipad somewhere using ifuse, say /media

    ifuse /media

Then you can begin transferring like this

    book2pad -d /media ~/doc/\*.pdf

``-d mountpoint`` indicates where the ipad is mounted. If omitted, the current working directory will be treated as the mountpoint.


Comments and bug reports
------------------------
Project page is on
https://github.com/rk700/rbook

You can also send email to the author:
`Ruikai Liu`_ 

.. _Ruikai Liu: lrk700@gmail.com
