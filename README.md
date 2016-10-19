Infrastructure Manager client
=============================

The ansible role deploys the Infrastructure Manager (IM) client tool.

* https://github.com/grycap/im-client

Role Variables
--------------

Variables for the im_client.cfg configuration file, see configuration
section in https://github.com/grycap/im-client:

* xmlrpc_url: http://localhost:8899
* auth_file: auth.dat
* xmlrpc_ssl: no
* xmlrpc_ssl_ca_certs: /tmp/pki/ca-chain.pem

Variables for the auth.dat authorization file:

* keystone_url: http://kystone:5000
* username: user
* passwd: pass
* tenant: proj
* iam_token: some_access_token

Example Playbook
----------------

```
---
- hosts: localhost
  roles:
    - indigo-dc.im-client
```

License
-------

Apache v2

Author Information
------------------

Mario David: <mariojmdavid@gmail.com>

LIP Lisbon: http://www.lip.pt

Indigo DataCloud: https://www.indigo-datacloud.eu/

Acknowledgments
---------------

Team at Grid y Computación de Altas Prestaciones (GRyCAP),
Universidad Politécnica de Valencia (UPV).

* http://www.grycap.upv.es/
* http://www.grycap.upv.es/im/