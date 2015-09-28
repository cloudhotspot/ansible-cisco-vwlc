# Automating Deployment of Cisco vWLC on VMWare Fusion

This Ansible playbook can be used to automate deployment of the Cisco Virtual Wireless LAN Controller (vWLC) on VMWare Fusion.

This has been tested on the following system:

- OS X 10.10.5 (Yosemite)
- VMWare Fusion 7.1.2
- Ansible 1.9.3
- Cisco vWLC version 8.0.120.0

## Prerequisites

- Mac OS X
- <a href="http://www.vmware.com/products/fusion" target="_blank">VMWare Fusion</a> 7.x or higher
- <a href="https://www.vmware.com/support/developer/ovf/" target="_blank">VMWare OVF Tools</a> 4.1 or higher (VMWare account may be required)
- <a href="http://www.ansible.com/" target="_blank">Ansible 1.9.x or higher
- <a href="https://software.cisco.com/download/release.html?mdfid=284464214&softwareid=280926587&release=8.0.120.0&relind=AVAILABLE&rellifecycle=ED&reltype=latest" target="_blank">Cisco vWLC OVA Image</a> (CCO login required)

This playbook also relies on the Ansible Galaxy <a href="https://github.com/yaegashi/ansible-role-blockinfile" target="_blank">yaegashi.blockinfile module</a>.  You must install this module prior to running the playbook:

```bash
$ansible-galaxy install yaegashi.blockinfile
- downloading role 'blockinfile', owned by yaegashi
- downloading role from https://github.com/yaegashi/ansible-role-blockinfile/archive/v0.5.tar.gz
- extracting yaegashi.blockinfile to /usr/local/etc/ansible/roles/yaegashi.blockinfile
- yaegashi.blockinfile was installed successfully
```