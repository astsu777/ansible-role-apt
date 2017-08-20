Ansible Role: APT
=========

This role configure the aptitude package on Debian system. It enables automatic installation of security updates and provide email notification as soon as a package update is available.

Requirements
------------

No specific requirements for this role.

Role Variables
--------------

The only variable for this role is the email address used for the notifications. It can be configured like this:

``` apt_email_address: myemail@email.com ```

The variable can be defined in group_vars or in host_vars.

Dependencies
------------

No dependencies from other roles required.

Example Playbook
----------------

Here is a simple example playbook to use this role:

```
hosts: all
user: root
roles:
  - { role: apt, tags: [ 'apt' ] }
```

License
-------

MIT / BSD

Author Information
------------------

My name is Gaétan. You can follow me on [Twitter](https://twitter.com/gaetanict)

Website: [ICT Pour Tous](https://www.ictpourtous.com)
