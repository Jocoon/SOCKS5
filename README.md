SOCKS5
======

A PHP5 Library to make TCP connections via a SOCKS5 Proxy.

It will create a standard socket which can be used with the normal functions like
fwrite(), fgets(), etc. Just be aware the connection is non-blocking.

Important Note
------------

This library has been modified to use a blocking connection
in contrast to the original library by weheartwebsites / Günter Grodotzki.
By the way, this library has been tested up to PHP 7.2 and it works flawlessly.


Requirements
------------

* PHP5.4 or higher


Features
--------

* ability to set the outgoing interface (e.g. multi-ip environments)
* ability to tunnel DNS over the Proxy as well, or do DNS queries local
    * for example if the DNS server is trustable (like a local cache) it might
      be faster to do the DNS query directly than over the Proxy
* minimal requirements, created socket can be used transparently with PHP built
  in functions.
* for now, plaintext authentication implemented
