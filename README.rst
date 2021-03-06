=======
org-tfl
=======

Use the Transport For London API in Emacs, powered by helm and org-mode.

This is an experimental project to use the `Transport for London (TfL) API <https://api-portal.tfl.gov.uk/docs>`_ in combination with Emacs orgmode.

.. CAUTION:: This is a very hacky software, written by a complete lisp newbie.
	     The author is aware that the code is ugly, bad, dangerous
	     and needs a lot of work.

Installation
------------

It's available on `MELPA <https://melpa.org>`_.

Add the following to your emacs init file::

  (require 'org-tfl)

Screencast
----------

.. figure:: https://raw.github.com/storax/org-tfl/master/screencast1.gif

   Plan a journey and inspect the result in a buffer.
   View maps via google static maps.

.. figure:: https://raw.github.com/storax/org-tfl/master/screencast2.gif

   Plan a journey and create a special link in org-mode.
   Loading the link will refresh the result.

Commands
---------

Below are complete command list:

* ``org-tfl-jp``
   Plan a journey and view the result in a buffer.
* ``org-tfl-jp-org``
   Plan a journey and insert a subheading with a special link.
   The content is the journey result. Open the link to update it.
   Use the scheduling function of org mode to change the date.
   All other options are set via properties.

Customizable Options
---------------------

Below are customizable option list:

* ``org-tfl-api-id``
  Your Application ID for the TfL API. You don't need one
  for personal use. It's IP locked anyway.
* ``org-tfl-api-key``
  Your Application KEY for the TfL API. You don't need one
  for personal use. It's IP locked anyway.
* ``org-tfl-map-width``
  The width in pixels of static maps.
* ``org-tfl-map-height``
  The height in pixels of static maps.
* ``org-tfl-map-type``
  The map type. E.g. "roadmap", "terrain", "satellite", "hybrid".
* ``org-tfl-map-path-color``
  The color of the path of static maps.
* ``org-tfl-map-path-weight``
  The storke weight of paths of static maps.
* ``org-tfl-map-start-marker-color``
  The path color of static maps.
* ``org-tfl-map-start-marker-color``
  The start marker color of static maps.
* ``org-tfl-map-end-marker-color``
  The end marker color of static maps.
* ``org-tfl-time-format-string``
  The format string to display time.
* ``org-tfl-date-format-string``
  The format string to display dates.
