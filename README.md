Ansible Display
=============

This is the Display implementation of Ansible. It runs a series of tasks designed to set the expected state in Ansible.

Customization
-------------

If there are tasks that are specific to this property, create roles for them. If the tasks can be used, create them in
another repository, and add that repository as a submodule to this one

Execution Instruction
---------------------

The following command will execute the playbook:

```
$ ansible-playbook -i inventory display.yml
```

Authentication is handled out of band; it assumes that the user will have the appropriate `${HOME}/.ssh/config` file
set up. Such a file will look something like the following:

```
Host dp
    User display
    IdentityFile path/to/the/private/key.pem
```

Contact: hello@andrewhowden.com
Web:     https://www.andrewhowden.com/
