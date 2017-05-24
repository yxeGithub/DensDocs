.. |labmodule| replace:: 2
.. |labnum| replace:: 1
.. |labdot| replace:: |labmodule|\ .\ |labnum|
.. |labund| replace:: |labmodule|\ _\ |labnum|
.. |labname| replace:: Lab\ |labdot|
.. |labnameund| replace:: Lab\ |labund|

REST
----------------------------------

Useful rest information

REST Commands
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#.  Here is the first rest command

.. code:: rest

   curl -sk -u admin:password https://bigip.domain.com/mgmt/tm/ltm/pool -H "Content-Type: application/json" | sed 's/,/\'$'\n/g'
