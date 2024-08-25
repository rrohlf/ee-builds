# ee-builds
Repo for custom EE builds using ansible-builder

Ansible-builder basics

Install ansible-builder using the RH repo provided package. Two examples. One based on that you have the AAP repo available either from Red Hat's CDN or sourced from a Red Hat Satellite provided AP repo:
# dnf --enablerepo=ansible-automation-platform-2.4-for-rhel-8-x86_64-rpms install ansible-builder -y

This example is based on using the AAP "bundle" (offline) installer on a node that the installer has previously run on. You can verify the existance of the local bundle repo by listing the contents of the /etc/yum.repos.d/ directory and looking for the "ansible-automation-platform.repo" file.
dnf --enablerepo=ansible-automation-platform install ansible-builder -y

Usage instructions can be found at the following links:
https://docs.redhat.com/en/documentation/red_hat_ansible_automation_platform/2.4/html-single/creating_and_consuming_execution_environments/index#con-building-definition-file.
https://ansible.readthedocs.io/projects/builder/en/latest/
