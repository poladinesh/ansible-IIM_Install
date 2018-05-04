# ansible-IIM_Install

About:

This ansible playbook will install IBM Installation manager. Works only on RedHat Machines. Tested on Centos 7
Installation Directory: /opt/IBM/InstallationManager
This playbook is written for local purposes. Will be adding another file shortly which can be used for remote installs too.

How to use this:

ansible-playbook IIM_Install.yaml

Pre-Requisities: 

Download the IBM Installation Manager Zip file and copy it to /tmp location


Sample Output:
[root@localhost tmp]# ansible-playbook IIM_Install.yaml
 [WARNING]: Could not match supplied host pattern, ignoring: all

 [WARNING]: provided hosts list is empty, only localhost is available


PLAY [127.0.0.1] *******************************************************************************************************


TASK [Gathering Facts] *************************************************************************************************

ok: [127.0.0.1]

TASK [Update Yum-Repo] *************************************************************************************************

ok: [127.0.0.1]

TASK [Install pre-requisites] ******************************************************************************************

changed: [127.0.0.1] => (item=[u'unzip', u'java'])

TASK [Create Directory] ************************************************************************************************

changed: [127.0.0.1]

TASK [Unzip IBM Installation Manager] **********************************************************************************

changed: [127.0.0.1]

TASK [Install IBM Installation Manager] ********************************************************************************

changed: [127.0.0.1]

PLAY RECAP *************************************************************************************************************

127.0.0.1                  : ok=6    changed=4    unreachable=0    failed=0
