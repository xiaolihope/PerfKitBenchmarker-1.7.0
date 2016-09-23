#Install PerfKit
```bash
$ cd /path/to/PerfKitBenchmarker
$ sudo pip install -r requirements.txt
```
#Install OpenStack CLI client and setup authentication
```bash
$ sudo pip install -r perfkitbenchmarker/providers/openstack/requirements.txt
$ cat openrc
export OS_PROJECT_DOMAIN_ID=default
export OS_USER_DOMAIN_ID=default
export OS_PROJECT_NAME=admin
export OS_TENANT_NAME=admin
export OS_USERNAME=admin
export OS_PASSWORD=c605bc305a7ea1dc64d4
export OS_AUTH_URL=http://159.122.194.137:5000/v3
export OS_IDENTITY_API_VERSION=3

```
#Running a Single Benchmark
```bash
1) ./pkb.py --openstack_private_network='test-net' --openstack_public_network='Private-Network' --cloud=OpenStack --machine_type=m1.medium --openstack_network='test-net' --benchmarks=block_storage_workload --image='xenial-ubuntu-new'

2) ./pkb.py --openstack_private_network='test-net' --openstack_public_network='Private-Network' ----openstack_network=test-net  --openstack_floating_ip_pool='Private-Network' --cloud=OpenStack --benchmarks=ping
```
#Running speccpu2006
```bash

```
