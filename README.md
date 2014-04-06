# thttpd - tiny HTTP server

thttpd is a simple, small, portable, fast, and secure HTTP server.

Simple: It handles only the minimum necessary to implement HTTP/1.1.

Small: It has a very small run-time size, since it does not fork and is very
careful about memory allocation.

Secure: It goes to great lengths to protect the web server machine against
attacks and breakins from other sites.

It also has URL-traffic-based throttling.

See the manual entry for more details. See the INSTALL file for
configuration and installation instructions.

usage :
    ./configure 
    make


test.config :

port=80
user=nobody
dir=./www
nochroot
cgipat=/cgi-bin/**
logfile=thttpd.log
pidfile=thttpd.pid

Original author:
    Jef Poskanzer  jef@mail.acme.com  http://www.acme.com/jef/
