README for book2pad
===================

book2pad is a simple script for transferring books(PDF or EPUB) from linux machine to ipad. Jailbreaking is not needed. Tested working with iOS 8.3, 9.1.

Requirements
------------

* install `ifuse <http://www.libimobiledevice.org>`_ on your computer
* install python libraries:
    hashlib
    shutil
    argparse
    traceback
    pyexifinfo
    zipfile
    biplist
    binaryornot

  simply run this:

    pip install hashlib shutil argparse traceback pyexifinfo zipfile biplist binaryornot

Usage
-----

First, I want to recommend this library structure: [your_library](https://github.com/qunxyz/book2pad/tree/master/your_library). This script would tried to read title and author from book's metadata, otherwise would tried to parse filename.

If the iPad's contents don't show up immediately after plugging in, mount your ipad somewhere using ifuse, say /media

    ifuse /media

Then you can begin transferring like this, directory name will be as genre

    book2pad -d /media -b ~/doc/

    book2pad -d /media -b ~/doc/file.pdf

    book2pad -d /media -b ~/doc/file.pdf ~/doc/others


``-d mountpoint`` indicates where the ipad is mounted. If omitted, the current working directory will be treated as the mountpoint.


Comments and bug reports
------------------------
Project page is on
https://github.com/rk700/rbook

You can also send email to the author:
`Ruikai Liu`_ 

.. _Ruikai Liu: lrk700@gmail.com
