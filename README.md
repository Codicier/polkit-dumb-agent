polkit-dumb-agent
-----------------

polkit is dumb, and never works.

so here is probably the simplest version you can have (except the first one
that just ACKed every call), 99 lines of C++ and 46 lines of C.

it just uses kdesu to call a helper as root to send the reply, so all requests
requires the user to enter the root password.


TODO
----

Write a simple replacement for polkit itself, it's a simple dbus API and
90% of what it provides is never used.


Requirements
------------

 - C++ compiler
 - Qt5 (dbus and widgets)
 - kdesu