Create web document root
========================

This Ansible role will create the initial document root for a web app.

Role Variables
--------------

None.

Example requirements.yml
------------------------

```yml
---

- src: git+git@code.siftware.com:ansible/create-web-document-root.git
  version: "1.0"
  name: siftware.create-web-document-root
```

Example Playbook
----------------

An example playbook of how to use the role.

```yaml
---

- hosts: all
  roles:
  - siftware.create-web-document-root
```

License
-------

MIT

Author Information
------------------

Written by Iain Cuthbertson of [Siftware Ltd](http://siftware.com/)
