### Install Development version of Python, Python 3.10,

https://www.python.org/downloads/source/

`[anup@rhel-92-104 ~]$ sudo dnf install -y epel-release`

`[anup@rhel-92-104 ~]$ sudo dnf clean all`

`[anup@rhel-92-104 ~]$ sudo yum install gcc make bzip2-devel libffi-devel -y`

`[anup@rhel-92-104 ~]$ sudo yum groupinstall "Development Tools" -y`

<br>

`[anup@rhel-92-104 ~]$ wget https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tgz`

`[anup@rhel-92-104 ~]$ ls -ltr`

`[anup@rhel-92-104 ~]$ tar -xvzf Python-3.10.13.tgz `

`[anup@rhel-92-104 ~]$ cd Python-3.10.13/`

<br>

`[anup@rhel-92-104 Python-3.10.13]$ ./configure --prefix=/usr/local/Python-3.10.13`

<br>

`[anup@rhel-92-104 Python-3.10.13]$ make`

`[anup@rhel-92-104 Python-3.10.13]$ sudo make install`

`[anup@rhel-92-104 Python-3.10.13]$ /usr/local/Python-3.10.13/bin/python3 --version`

`[anup@rhel-92-104 Python-3.10.13]$ export PATH="/usr/local/Python-3.10.13/bin:$PATH"`

<br>

`[anup@rhel-92-104 Python-3.10.13]$ python3.10 --version`

`[anup@rhel-92-104 Python-3.10.13]$ python3 --version`

`[anup@rhel-92-104 Python-3.10.13]$ compgen -c python | grep -P '^python\d'`

`[anup@rhel-92-104 Python-3.10.13]$ ls -1 /usr/bin/python* | grep '.*[2-3]\(.[0-9]\+\)\?$'`

`[anup@rhel-92-104 Python-3.10.13]$ ls -l /usr/bin/python*`


### Change the default version,

`[anup@rhel-92-104 Python-3.10.13]$ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.10.13 1`

`[anup@rhel-92-104 Python-3.10.13]$ sudo update-alternatives --display python3`

`[anup@rhel-92-104 Python-3.10.13]$ python3 --version`

<br>
