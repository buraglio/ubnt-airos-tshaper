# ubnt-airos-tshaper
## What
Ansible playbooks to enable and configure the traffic shaper on Ubiquity AirOS CPE
## Why?
Ubiquity radios don't seem to have a way to push out mass changes to the tshaper. This stinks, because using the GUI at scale just doesn't work. Until their tools like UNMS or others allow for mass changes to the tshaper settings, this pile of ansible will have to do. 

## How
These CPE radios are painful to make automated changes on, and there currently is no ansible module to do it, so it seemingly has to use raw. 
You'll need to install ansible. Place the files in the folders they are currently in and run the command

`ansible-playbook /etc/ansible/playbooks/ubnt-airos-tshaper.yml`

## To Do
Clean up some of the code. There are more efficient ways to set the rates (i.e. variables), and that should be done. I am by no stretch of the imagination an Ansible expert, so if there are better ways to do this, feel free - and encourages - to submit patches. 

## other stuff
*Use anything I write at your own peril.* 
