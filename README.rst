|debops_logo| `DebOps <http://debops.org>`_
===========================================

**Your Debian-based data center in a box**

A collection of `Ansible <http://ansible.com/>`_ playbooks,
scalable from one container to an entire data center.

DebOps is a framework
^^^^^^^^^^^^^^^^^^^^^

- **50+ highly extensible roles** with sane defaults
- **Tuned for production** and works great for development
- **Built for modularity** so extending it is simple
- **Custom scripts** to tie everything together

We believe in the UNIX philosophy; one tool should only do one thing very well.
DebOps has many playbooks and roles but it is just a set of focused tools to
help you run and manage your infrastructure.

In fact all of the DebOps playbooks and roles can be ran with Ansible directly.

Installation
^^^^^^^^^^^^

::

   $ git clone https://github.com/debops/debops
   $ cd debops ; sudo make install

Getting started
^^^^^^^^^^^^^^^

**Make your first project**

::

   $ debops-init ~/myproject

**Add a host to your inventory**

Take a peek at ``~/myproject/ansible/inventory/hosts``.

**Verify it**

::

   $ ssh yourhost
   $ debops-task all -m setup

**Run the DebOps playbooks**

::

   $ debops

What do you want to learn more about?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

|Gratipay|_

- `Playbooks and roles <https://github.com/debops/debops-playbooks>`_
- `Custom scripts <https://github.com/debops/debops/blob/master/doc/using-the-custom-scripts.rst>`_
- `How will versions work with so many roles and playbooks? <https://github.com/debops/debops/blob/master/doc/versions.rst>`_
- DebOps guides and troubleshooting
    - `Using linux containers <https://github.com/debops/debops/blob/master/doc/using-linux-containers.rst>`_
    - `Creating a local APT server to use backports <https://github.com/debops/debops/blob/master/doc/creating-a-local-apt-server-to-use-backports.rst>`_
    - `Solving common problems <https://github.com/debops/debops/wiki/Solutions-to-problems-you-may-encounter>`_

Do you want to contribute?
^^^^^^^^^^^^^^^^^^^^^^^^^^

Sounds great, check out the `contributing guide <https://github.com/debops/debops/blob/master/CONTRIBUTING.rst>`_
for the details.

Authors
```````

**Maciej Delmanowski**

- Email: drybjed@gmail.com
- Twitter: `@drybjed <https://twitter.com/drybjed>`_
- Github: `drybjed <https://github.com/drybjed>`_

**Nick Janetakis**

- Email: nick.janetakis@gmail.com
- Twitter: `@nickjanetakis <https://twitter.com/nickjanetakis>`_
- Github: `nickjj <https://github.com/nickjj>`_

.. |Gratipay| image:: https://img.shields.io/gratipay/drybjed.svg?style=flat
.. _Gratipay: https://www.gratipay.com/drybjed/
.. |debops_logo| image:: http://debops.org/images/debops-small.png