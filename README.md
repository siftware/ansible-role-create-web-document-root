Create web document root
========================

This Ansible role will create the initial document root for a web app.

Role Variables
--------------

```yaml
base_dir: /var/www/project
releases_directory: "{{ base_dir }}/releases"
current_symlink_name: current
relative_document_root: codebase/public
web_document_root_user: www-data
web_document_root_group: www-data
```

Example requirements.yml
------------------------

```yaml
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
