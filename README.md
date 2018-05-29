Jenkins
========

This is an ansible role to install Jenkins on server.

Usage
--------
```
ansible-playbook deploy.yml -vvv -e"extravarkey=extravarvalue"
```

Variables
---------

### Default Variables

* `jenkins_port` -- The port Jenkins listens on. (Default `8080`).

* `jenkins_url` -- Jenkins URL.




Other Information
-----------------

### Reload Handler
We have used the `url` module in the reload handler, because its the safe restart option for Jenkins and will wait until all current tasks are finished before restarting the service.


Bug Reports
-----------

Bug reports can be directly sent to authors and/or using github's issues.


Author Information
------------------

Utkarsh Sharma <utkarshredhat@gmail.com>
