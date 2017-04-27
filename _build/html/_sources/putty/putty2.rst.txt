.. |labmodule| replace:: 2
.. |labnum| replace:: 1
.. |labdot| replace:: |labmodule|\ .\ |labnum|
.. |labund| replace:: |labmodule|\ _\ |labnum|
.. |labname| replace:: Lab\ |labdot|
.. |labnameund| replace:: Lab\ |labund|

Plink
----------------------------------

Plink is for automating putty commands

Plink Commands
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#.  This command will license the bigip:
    `"C:\Program Files\PuTTY\plink.exe" -l admin -pw admin 10.1.1.7 run /util bash -c \"/usr/local/bin/SOAPLicenseClient --basekey J1701-07024-25118-65122-2084674\"`

#.  This command will login to the bigip and change the password to what is in the master-key.txt file:
    `"C:\Program Files\PuTTY\plink.exe" -l admin -pw admin 10.1.1.7 run /util bash -c \"sh load-ucs.sh\"`

    load-ucs.sh

    ::

	   cat master-key.txt |tmsh modify /sys crypto master-key prompt-for-password
	   tmsh save /sys config
	   tmsh load /sys ucs initial-config.ucs no-license

    master-key.txt

    ::

	   default
	   default

#.  This command will run "C:\Program Files\PuTTY\plink.exe" -load automation "./run-demo.sh".  This is a linux box that has the GitHub repository on it and it runs the file - run-demo.sh

#.  This command will run "C:\Program Files\PuTTY\plink.exe" -load automation ./test.sh.  This is a linux box that has the GitHub repository on it and it runs the file - test.sh
