---
- name: Install Apache2 and Nginx
  hosts: all
  become: true
  tasks:
    - name: Install Apache2 on EC2 instance with Apache tag.
      yum:
        name: httpd
        state: present
      when: "'apache' in group_names"

    - name: Install Nginx on EC2 instance with Nginx tag
      yum:
        name: nginx
        state: present
      when: "'nginx' in group_names"
