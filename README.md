NFS on Kubernetes Example
=========

This is an ansibilization of an example from the following repo:
https://matthewpalmer.net/kubernetes-app-developer/articles/kubernetes-volumes-example-nfs-persistent-volume.html

Requirements
------------

- A working kubernetes cluster to run ansible against.

Role Variables
--------------

nfs_cluster_state: ['absent', 'present']

Dependencies
------------

Not dependent on any other roles.  

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: kube-master[0]
      become: True
      roles:
        - role: senorsmile.k8s-nfs
          tags:
            - k8s
            - nfs

License
-------

BSD

Author Information
------------------

Shaun Smiley (senorsmile)
