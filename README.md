win_inet_pton
=============

Native inet_pton and inet_ntop implementation for Python on Windows (with ctypes).


Credit Where Credit Is Due
--------------------------

This package is based on code that was originally written by https://github.com/nnemkin here: https://gist.github.com/nnemkin/4966028


Why?
----

I needed this functionality in https://github.com/SerenitySoftwareLLC/cahoots to get full windows support. I figured, since there were other people looking for a solution to this on the net, I should publish it.


Usage
-----

```pip install win_inet_pton```

Just import it, and it will auto-add the methods to the socket library:
```
import win_inet_pton
import socket

socket.inet_pton(...)
socket.inet_ntop(...)
```