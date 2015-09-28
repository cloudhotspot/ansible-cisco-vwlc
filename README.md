# Automating Deployment of Cisco vWLC on VMWare Fusion

This Ansible playbook can be used to automate deployment of the Cisco Virtual Wireless LAN Controller (vWLC) on VMWare Fusion

## Prerequisites

This playbook relies on the Ansible Galaxy <a href="https://github.com/yaegashi/ansible-role-blockinfile" target="_blank">yaegashi.blockinfile module</a>.  You must install this module prior to running the playbook:

`ansible-galaxy install yaegashi.blockinfile`