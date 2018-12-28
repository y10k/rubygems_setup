rubygems_setup
=========

Setup gems for all users.

Requirements
------------

None.

Role Variables
--------------

| Variable | Default | Description |
|----------|---------|-------------|
|`rubygems_setup_state`|`present`|it is the same as the `state` of `gem` module|
|`rubygems_setup_document`|`yes`|it is the same as the `include_doc` of `gem` module|
|`rubygems_setup_list`|`bundler`|List of gems to be set up.|

Dependencies
------------

- `y10k.rubygems_environment`

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: y10k.rubygems_setup
```

License
-------

BSD
