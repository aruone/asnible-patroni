Requested Features
------------------

* Add support of Consul and ZooKeeper.
* Support of post init/bootstrap scripts that will be executed after initializing the cluster.
* Support of callback scripts to run on certain actions (on_reload/on_restart/on_role_change/on_start/on_stop).
* Support of user-defined scripts to bootstrap new clusters (bootstrap.method configuration setting).
* Manage SSL certificates for DCS and Patroni REST API.
* Support of different PostgreSQL replication modes (synchronous/cascading replication).
* Make cross-platform compatible.
* Integrate with [Travis CI](https://travis-ci.org/).
* Support of custom replica creation methods via 3rd party tools like Barman, WAL-E, pgBackRest.

Known Issues
------------

* PostgreSQL service is required to be disabled at boot time while controlled via patroni.
* No support of rpm-based Linux distros and Ubuntu < 16.04.
* replica_method, recovery_conf, callbacks, post_init, post_bootstrap, patroni_etcd_* parameters are not setting properly.