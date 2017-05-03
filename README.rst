This is a fork of the django web application framework, patched specifically
for https://github.com/frePPLe/frePPLe.  FrePPLe users should install this
patched version of django.

Every frePPLe release has a seperate branch in this repository to provide
full tracebility of all changes.

At a high level the patch addresses the following topics:

* Database routing that is controlled with a URL prefix.
  For instance:
    http://host/data/admin/1 uses the 'default' database.
    http://host/copy1/data/admin/2 uses the 'copy1' database.
    http://host/copy2/data/admin/2 uses the 'copy2' database.

* Autoreload fix to keep working when using a py2exe executable.

* Admin edit form doesn't display the current value after
  the control.

* Minor corrections to support multiple admin sites.

* Adding request variable to the template context.

-----------------------------------------------------------------------------

Django is a high-level Python Web framework that encourages rapid development
and clean, pragmatic design. Thanks for checking it out.

All documentation is in the "``docs``" directory and online at
https://docs.djangoproject.com/en/stable/. If you're just getting started,
here's how we recommend you read the docs:

* First, read ``docs/intro/install.txt`` for instructions on installing Django.

* Next, work through the tutorials in order (``docs/intro/tutorial01.txt``,
  ``docs/intro/tutorial02.txt``, etc.).

* If you want to set up an actual deployment server, read
  ``docs/howto/deployment/index.txt`` for instructions.

* You'll probably want to read through the topical guides (in ``docs/topics``)
  next; from there you can jump to the HOWTOs (in ``docs/howto``) for specific
  problems, and check out the reference (``docs/ref``) for gory details.

* See ``docs/README`` for instructions on building an HTML version of the docs.

Docs are updated rigorously. If you find any problems in the docs, or think
they should be clarified in any way, please take 30 seconds to fill out a
ticket here: https://code.djangoproject.com/newticket

To get more help:

* Join the ``#django`` channel on irc.freenode.net. Lots of helpful people hang
  out there. See https://en.wikipedia.org/wiki/Wikipedia:IRC/Tutorial if you're
  new to IRC.

* Join the django-users mailing list, or read the archives, at
  https://groups.google.com/group/django-users.

To contribute to Django:

* Check out https://docs.djangoproject.com/en/dev/internals/contributing/ for
  information about getting involved.

To run Django's test suite:

* Follow the instructions in the "Unit tests" section of
  ``docs/internals/contributing/writing-code/unit-tests.txt``, published online at
  https://docs.djangoproject.com/en/dev/internals/contributing/writing-code/unit-tests/#running-the-unit-tests
