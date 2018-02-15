Role Name
=========

This role installs pip using easy_install only when using a Debian distribution

Requirements
------------

None really, but this will only work with distro = debian. With other distros this role will do nothing.

Role Variables
--------------

In case you want packages to be installed by pip, you can also do that with this variable like this: 

    pip_install_packages:
      # Test installing damn pyOpenSSL.
      - name: pyOpenSSL
        version: "17.5.0"

Dependencies
------------

None

Example Playbook
----------------

Is there a way to change my name to lower case from github? :S

    - hosts: all
      roles:
         - { role: FrancescJR.debian-pip }

License
-------

MIT whatever, this is already half copied from Geerlingguy's role. But somehow I could not install pyOpenSSL if
pip was installed via apt on Debian, cause pip version would be so outdated. That's why I did this.

Author Information
------------------

Not really into computer stuff, I like more languages and sports but programming gives me more money. 
I do really like a lot Ansible though and devops in general. I am impressed by Geerlingguy.

