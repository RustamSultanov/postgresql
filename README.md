PostgreSQL 10 for CentOS 7
=========

Installs and configures PostgreSQL 10 server on CentOS7


Requirements
------------

Only root access

Role Variables
--------------

Defaults: `defaults/main.yml`

- `postgres_conf_listen_addresses`: What IP address(es) to listen on
- `postgres_conf_shared_buffers`: Sets the amount of memory the database server uses for shared memory buffers (min 128kB)
- `postgres_conf_work_mem`: Specifies the amount of memory to be used by internal sorts and hashes before resorting to temporary disk files (min 64kB)
- `postgres_conf_max_connections`: The maximum number of concurrent connections to the database server

- `postgres_init_db_name`: Database name
- `postgres_init_user_name`: Database user name
- `postgres_init_user_password`: Database user password

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - tfs-devops-postgres


Author Information
------------------

Rustam Sultanov

