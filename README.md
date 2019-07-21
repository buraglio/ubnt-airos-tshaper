# ubnt-airos-tshaper

## What?
Ansible playbook to enable and configure the traffic shaper on Ubiquity AirOS CPE. 
## Why?
Ubiquity radios don't seem to have a way to push out mass changes to the tshaper. This stinks, because using the GUI at scale just doesn't work. Until their tools like UNMS or others allow for mass changes to the tshaper settings, this pile of ansible will have to do. Best practice is to rate limit on the devices closest to the customer. Some people don't use RADIUS or PPPoE to do the things, this aids in performing that specific task in the WISP industry

## How?
These CPE radios are painful. They're painful to manage. They're painful to operate. They're painful to make any mass changes on. They're painful to make automated changes on. *but* they're inexpensive and *extremely* pervasive. They mostly work as advertised. There currently is no ansible module to do it, so it seemingly has to use raw. 
You'll need to install ansible. Place the files in the folders they are currently in and run the command

`ansible-playbook /etc/ansible/playbooks/ubnt-airos-tshaper.yml`

## To Do
Clean up some of the code. There are more efficient ways to set the rates (i.e. variables), and that should be done. I am by no stretch of the imagination an Ansible expert, so if there are better ways to do this, feel free - and encouraged - to submit patches. 

## other stuff
*Use anything I write at your own peril.* 

Thanks to [Sam Oehlert](https://github.com/soehlert) for helping teach me the fundamentals. 

Sometimes I put stuff on my [website](https://www.forwardingplane.net). You can contact me via [email](mailto:buraglio@forwardingplane.net) or [Twitter](https://www.twitter.com/buraglio) or [LinkedIN](https://www.linkedin.com/in/buraglio/). I'm not always responsive in a timely manner and probably won't be able to help you do ansible stuff, but generally do eventually reply.   
