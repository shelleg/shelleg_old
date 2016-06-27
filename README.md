shelleg
=======

Synopsis:
--------
The central place where integration of shlleg CM happens.
This repository will integrate the various mooving parts of the [Shelleg project](http://shelleg.github.io/shellegDoc/Intro.html)

Repo Structure:
--------------

``` shell
.
├── LICENSE                      # TBD project final license
├── README.md                    # this file
├── ansible                      # Ansible implementation
│   ├── ansible.cfg              # Ansible config file
│   ├── inventories              # Ansible inventories [ static | ec2 | openstack etc ]
│   ├── log                      # Log directory placeholder
│   │   └── ansible.log          # Only in initial structure, it will remain in .gitignore ...
│   ├── playbooks                # Ansible Playbooks directory
│   │   ├── group_vars           # Ansible group variables see ./all below
│   │   │   └── all              # A folder which can store a hierarcy of ansible vars
│   │   └── host_vars            # Place for host specific variables
│   ├── roles                    # Ansible external roles directory
│   └── site-roles               # Internally developed roles directory in case we need it ...
└── bin                          # will store and scripts / functions we may need 
└── requirements.yml             # Dependency management of Ansible roles see file;s internal comments
```

Shellg Resources
----------------

* [ShellgDocs](http://shelleg.github.io/shellegDoc/)
* [Issues](https://github.com/shelleg/shelleg/issues)
* Please note: role specific issues should be files in the role level
