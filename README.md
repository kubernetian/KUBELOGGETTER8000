# KubeLogGetter8000

![KUBELOGGETTER8000](mediafiles/kubeloggetter8000.jpg)


# Introduction 

Hi, I'm joris and I'm sick and tired of typing : 

    -f --tail 50

# Prerequisites 

No prereqs apart from having a kubernetes cluster? 

# How to install? 

Simple tools for smart minds. Do the following steps : 
* Clone this git 
* Put the KLG8 file in your `/usr/local/bin` folder
* Edit the permissions on the file `chmod +x /usr/local/bin/KLG8`
* `exec $SHELL` (Optional step, re-opening your terminal will do the trick as well) 
* You will be able to use `KLG8` as a command from now on

## BEST INSTALLATION STEP 

Wait for the .deb package you lazy fish. 
# Example 

        user@ubuntu:~# KLG8 -n kube-system
        1) coredns-66bff467f8-5wv8z	     5) kube-controller-manager-minikube
        2) coredns-66bff467f8-9hhj6	     6) kube-proxy-5ngks
        3) etcd-minikube		     7) kube-scheduler-minikube
        4) kube-apiserver-minikube	     8) storage-provisioner
        Which logs do you need? 3
        2021-12-10 13:29:10.943014 I | mvcc: store.index: compact 4976
        2021-12-10 13:29:10.945495 I | mvcc: finished scheduled compaction at 4976 (took 1.921691ms)
        2021-12-10 13:34:10.966779 I | mvcc: store.index: compact 5630
        2021-12-10 13:34:10.970809 I | mvcc: finished scheduled compaction at 5630 (took 3.258837ms)
        2021-12-10 13:39:10.978504 I | mvcc: store.index: compact 6282
        2021-12-10 13:39:10.980577 I | mvcc: finished scheduled compaction at 6282 (took 1.419146ms)
        2021-12-10 13:44:10.983319 I | mvcc: store.index: compact 6938
        2021-12-10 13:44:10.985339 I | mvcc: finished scheduled compaction at 6938 (took 1.248905ms)
        2021-12-10 13:49:10.990707 I | mvcc: store.index: compact 7588
        2021-12-10 13:49:10.992752 I | mvcc: finished scheduled compaction at 7588 (took 1.440962ms)
        2021-12-10 13:53:39.195273 I | etcdserver: start to snapshot (applied: 10001, lastsnap: 0)
        2021-12-10 13:53:39.202576 I | etcdserver: saved snapshot at index 10001
