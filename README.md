# virtstuff
Some basic virtualization with kvm.

A host has a lvs disk and a swap. 

Boot with direct kernel boot as 

```
  <os>
    <type arch='x86_64' machine='pc-q35-3.1'>hvm</type>
    <kernel>/var/lib/libvirt/images/vmlinuz-5.10.0-16-cloud-amd64</kernel>
    <initrd>/var/lib/libvirt/images/initrd.img-5.10.0-16-cloud-amd64</initrd>
    <cmdline>root=/dev/vda nohibernate noresume</cmdline>
    <boot dev='hd'/>
  </os>
```

## Create new host

Edit create-host ad exec

## Mirror / backup host

Edit lvs-mirror and exec
