### Install Python 3 and Set Up a Programming Environment, Python 3.9,

`[anup@rhel-92-104 ~]$ python --version`

`[anup@rhel-92-104 ~]$ python3 --version`

<br>

`[anup@rhel-92-104 ~]$ sudo yum groupinstall "Development Tools" -y`

`[anup@rhel-92-104 ~]$ sudo dnf install python3 -y`

<br>

### Installing and using Python,  Python 3.11,

https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html/installing_and_using_dynamic_programming_languages/assembly_installing-and-using-python_installing-and-using-dynamic-programming-languages

https://www.python.org/downloads/source/

`[anup@rhel-92-104 ~]$ python --version`

`[anup@rhel-92-104 ~]$ python3 --version`

<br>

`[anup@rhel-92-104 ~]$ sudo dnf -y groupinstall development`

`[anup@rhel-92-104 ~]$ sudo dnf install python3.11`

`[anup@rhel-92-104 ~]$ sudo update-alternatives --display python3`

`[anup@rhel-92-104 ~]$ python3.11 --version`

`[anup@rhel-92-104 ~]$ ls -1 /usr/bin/python* | grep '.*[2-3]\(.[0-9]\+\)\?$'`

<br>

### Change the default version,

`[anup@rhel-92-104 ~]$ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 1`

`[anup@rhel-92-104 ~]$ sudo update-alternatives --display python3`

`[anup@rhel-92-104 ~]$ python3 --version`

<br>


<br>
