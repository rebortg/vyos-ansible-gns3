Configuration Test with GNS3
==============

prepare
-------

*  install gns3-server
*  ```pip install -r requirements.txt```
*  install https://github.com/davidban77/ansible-collection-gns3

use it
------


```ansible-playbook lab_main.yml -e execute=create```

 1.  download the latest rolling iso
 2.  upload to gns3 server
 3.  create a new template
 4.  create a Project with nodes and links
 5.  boot the nodes
 6.  setup a IP and enable ssh


```ansible-playbook lab_main.yml -e execute=test```

 *  use the project from above
 *  setup internal interfaces
 *  perform a icmp test

```ansible-playbook lab_main.yml -e execute=delete```

 *  delete the project
 *  TODO: image and template cleanup