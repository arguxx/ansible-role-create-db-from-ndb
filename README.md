Role Name
=========

Role for provision DB via NDB

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

```yaml
---
# public data
# NDB config
ndb_ip: 
ndb_port: 
basic_auth: 
nx_cluster_id:
ssh_public_key:
clustered:

# Instance Settings
database_type: 
instance_name:
database_description:
softwareProfileId:
softwareProfileVersionId:
computeProfileId:
networkProfileId:
dbParameterProfileId:

# Time Machine settings
time_machine_description:
sla_id:

# Action Arguments
listener_port:
database_size:
auto_tune_staging_drive:
allocate_pg_hugepage:
cluster_database:
enable_peer_auth:
ensure_vm_host_distribution:
dbserver_description:
database_names:
db_password:

# nodes management
vm_name: 
network_profile_id:
vm_password:
```

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - { role: arguxx.create_db_from_ndb }
```
License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
