Zookeeper
=========

This is an ansible role that installs zookeeper on the given hosts. One can use the role by adding the following task in their playbook


Role Variables
--------------

| Variable               | default                                                                                  | description                                |
| -------------          | :-------------:                                                                          | -----:                                     |
| zookeeper_user         | zookeeper                                                                                | The user and group that will run zookeeper |
| zookeeper_binary       | https://downloads.apache.org/zookeeper/zookeeper-3.7.0/apache-zookeeper-3.7.0-bin.tar.gz | The url of the binary                      |
| zookeeper_data_path    | `/data/zookeeper`                                                                        | The path of the data dir                   |
| zookeeper_path         | `/opt`                                                                                   | The root of the installation               |
| zookeeper_http_enabled | true                                                                                     | Whether the http server should be enabled  |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

``` yaml
- name: Install zookeeper
  hosts: zookeeper
  roles:
    - role: zookeeper
      vars:
        zookeeper_http_enabled: false
```

License
-------

BSD
