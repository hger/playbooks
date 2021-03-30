# My example playbooks

These are purely for showcasing ansible tower

```
---
- hosts: all
  tasks:
  - name: Create the AD group travelers
    include_role:
      name: ad_group
    vars:
      ad_domain: fluxcapacitor.com
      ad_group_name: travelers
      ad_group_description: time travelers
      ad_group_ou: OU=school-teachers,OU=1885,DC=fluxcapacitor,DC=com
      ad_group_membership_users: ['emmett.brown@fluxcapacitor.com', 'marty.mcfly@fluxcapacitor.com']
```
