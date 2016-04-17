single-node-cloudconfig.yml:
cloud-config for single node CoreOS with etcd2, fleet, flannel services.
ssh key needs to be updated appropriately before using.

hademo/user-data can be used to start 3 node CoreOS cluster using Vagrant. Token needs to be updated.

Execute global service:
fleetctl start helloglobal.service

Execute HA Demo:
fleetctl submit apachet@.service apachet-discovery@.service
fleetctl start apachet@8080.service apachet-discovery@8080.service

