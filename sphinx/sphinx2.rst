.. |labmodule| replace:: 1
.. |labnum| replace:: 2
.. |labdot| replace:: |labmodule|\ .\ |labnum|
.. |labund| replace:: |labmodule|\ _\ |labnum|
.. |labname| replace:: Lab\ |labdot|
.. |labnameund| replace:: Lab\ |labund|

How to build documents
-------------------------------------------------------

To properly build Sphinx documentation you need to know a few things:

.. _formatting:

How to do formatting
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. To create a master heading use a bunch of ------ on a separate line

#. To create a subheading use a bunch of ~~~~ on a separate line

#. To create an ordered list (numbered) use the # symbol then a period.

#. To add an image via a variable use:

   ::

    |image12|

#. In this document I am using:

   ::

    - for top level
    ~ for sub headings


Variables for images
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This is another subheading and ordered list for variables

To create a variable for an image file to be used in a page do the following:

#.  Define the variable as such:

::

    .. |image8| image:: /_static/image008.png
    :width: 0.46171in
    :height: 0.43269in


Making Links
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It is easy to make a link to `yahoo <http://yahoo.com>`_ or to some
section inside this document (see :ref:`formatting`) or another
document.

To do this call something like this:

::

    Link to Yahoo = `yahoo <http://yahoo.com>`_

    Reference to a Page = see :ref:`task-1-formatting`
      You will also need to use .. _task-1-formatting: before your heading

You can also reference classes, modules, functions, etc that are
documented using the sphinx `autodoc
<http://sphinx.pocoo.org/ext/autodoc.html>`_ facilites.  For example,
see the module :mod:`matplotlib.backend_bases` documentation, or the
class :class:`~matplotlib.backend_bases.LocationEvent`, or the method
:meth:`~matplotlib.backend_bases.FigureCanvasBase.mpl_connect`.


.. |image12| image:: /_static/image012.png
   :width: 0.46171in
   :height: 0.43269in
