.. |labmodule| replace:: 3
.. |labnum| replace:: 1
.. |labdot| replace:: |labmodule|\ .\ |labnum|
.. |labund| replace:: |labmodule|\ _\ |labnum|
.. |labname| replace:: Lab\ |labdot|
.. |labnameund| replace:: Lab\ |labund|

Docker Basics
-------------------------

Install Docker for your OS - I am using a Mac so I downloaded and ran the Mac installer

List images
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

docker images

List containers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

docker ps -a

Run shell within a container
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

docker exec -it -u root jenkins-2 /bin/bash


.. |image66| image:: /_static/image066.png
   :width: 0.28045in
   :height: 0.24306in
.. |image67| image:: /_static/image067.png
   :width: 0.35694in
   :height: 0.30286in
.. |image68| image:: /_static/image068.png
   :width: 6.33450in
   :height: 0.81372in
.. |image69| image:: /_static/image069.png
   :width: 6.25116in
   :height: 0.51099in
