#### python -m venv virtualenv
d----          2/2/2023   4:07 PM                  virtualenv

#### Activate virtual env
 .\\Scripts\\activate
(virtualenv) "C:\\prg\\work\\virtualenv"

#### PIP requirements
![[pip requiriments]]



#### python.exe -m pip install --upgrade "pip < 21.0"
Collecting pip<21.0
  Using cached pip-20.3.4-py2.py3-none-any.whl (1.5 MB)
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 22.3.1
    Uninstalling pip-22.3.1:
      Successfully uninstalled pip-22.3.1
Successfully installed pip-20.3.4



### *Frontend*
**This folder is no longer in this branch**
1. `cd IRCPeopleDirectoryFrontEnd`

2. `ng serve` (will serve on http://localhost:4200/)

##### *Backend* (and compiled frontend)

1. `python manage.py runserver` (will serve on http://localhost:8000/)