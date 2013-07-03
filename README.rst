===============
tribaal-minimal
===============

What is tribaal-minimal?
------------------------

tribaal-minimal is a `pelican <http://getpelican.com>`_ theme based on the fantastic `Iris <https://github.com/slok/iris>`_, itself based on `Flask webpage <http://flask.pocoo.org/>`_ 

This theme is very simple and easy to read, perfect for a minimalist blog without much things and
beautiful source code syntax (thanks to `pygments <http://pygments.org/>`_!)

The main difference with Iris is that it uses the Ubuntu font almost everywhere instead of the original author's choice, as well as a few visal tweaks.

Preview
-------


Variables
---------

Some of the variables defined in this theme:

- ``DISQUS_SITENAME``: For the disqus comments
- ``EMAIL``: For the email "mailto:"

For the analytics we have two flavours, one is Go `Squared <https://www.gosquared.com>`_

- ``GOSQUARED_SITENAME``: For the Go squared analytics

And the other is `Google analytics <https://www.google.com/analytics>`_ Google analytics has various forms. The
basic one is:

- ``GOOGLE_ANALYTICS_CODE``: this is the code of GA, something similar to: ``UA-xxxxxxxx-y``

If you have analytics across domains you can put this setting:

- ``GOOGLE_ANALYTICS_DOMAIN = "xlarrakoetxea.org"``

And if you have upper domain level (com, org, co.uk...)

- ``GOOGLE_ANALYTICS_DOMAIN_UP = True``

Installation
------------

The easiest way to install a theme for pelican is to create a new themes directory
in you pelican project root and then checkout this repository into it::

    $ cd $my_pelican_project
    $ mkdir themes
    $ cd themes
    $ git clone https://github.com/chrisglass/tribaal-minimal

The pelican THEME variable can then be set to the following::

    THEME = "themes/tribaal-minimal"

Notes
-----

The theme navigation bar does a fade in if you scroll more than 300 pixels to
increase the readability of an article.

ReStructuredText creates ``tt`` with ````something```` that is equivalent to  markdown ``code``
that is created wit ```something```. This renders inline source code. So I added ``tt`` to the
css also, not only ``code`` like most themes. Example:


.. image:: https://raw.github.com/gist/3885420/4d7a8557780ab74c5ae797a4f6e82cbf11aec0c6/iris_inline.png
    :align: center

License
-------

This theme is under the `3 clause BSD license <http://opensource.org/licenses/bsd-3-clause>`_
