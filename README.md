# OpenStack test suite

This is a set of Ansible playbooks to exercise various features of an
OpenStack cloud.

## Requirements

Due to bugs in Ansible's OpenStack inventory plugin, you will need to
apply [PR #48833][] to your Ansible installation before you are able
to run these playbooks.

[pr #48833]: https://github.com/ansible/ansible/pull/48833

You can run an appropriate version of Ansible with the patch already
applied from a Python virtual environment by using the `pipenv` tool:

    $ pipenv install
    $ pipenv shell
    $ ansible-playbook playbook.yml
