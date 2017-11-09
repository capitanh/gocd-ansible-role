Role Name
=========

This role install go.cd Continous Delivery Server

Requirements
------------

This role requires ansible 2.4.0.0 or higher, platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows:

```yaml
    go_server_port: 8153  # Default http port
    go_server_ssl:  8154  # Default ssl listen port for agents
    go_pipelines_group    # go.cd pipelines group name
    go_environment        # go.cd initial configured environment
```

Dependencies
------------

None

Example Playbook
----------------

Register the role in requirements.yml:

```yaml
    - src: capitanh.gocd-ansible-role
      name: gocd
```
Include it in your playbooks:

```yaml
    - hosts: servers
      roles:
      - gocd
```

License
-------

BSD

