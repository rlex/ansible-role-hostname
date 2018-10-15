#### ansible role for setting hostname

Configures hostname RHEL-style, with FQDN in /etc/hostname.  
Also adds some essential records to /etc/hosts.  
By default it will take hostname specified in ansible inventory as default hostname.

##### Params
Following parameters are available (with default values):
```
hostname_hostname: "{{ inventory_hostname }}"
hostname_hostname_short: "{{ hostname_hostname.split('.')[0] }}"
hostname_ip_address: "{{ ansible_default_ipv4.address }}"
```
