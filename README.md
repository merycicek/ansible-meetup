# Ansible Meetup London Talk 
## How I save myself 30 minutes a day as a network engineer 

First delivered at the [Ansible London Meetup](https://www.meetup.com/Ansible-London/)

## Playbooks to backup Cisco routers and switches and push configurations and config templates
Does not work for NXOS but could easily be adjusted to hit NXOS or ASA by changing modules in use

## VIDEO 
Watch the video to see me walk you through these playbooks. 
https://youtu.be/MSp0eTDPDQE

## My Ansible Network Automation Course 
https://learn-network-automation.teachable.com/p/ansible-for-network-engineers

## Get started 
Clone the repo to your machine 

Change the hosts to addresses of your devices 

* `play1.yml` will just backup your devices 
* `play2.yml` will backup the devices in a date specific format and folder 
* `play3.yml` will backup devices 

To create Cisco configurations edit `/templates/roles/routers/templates/router.j2`
You can have your entire cisco configuration in here just add an `{{item.xxx}}` wherever you want a device specific variable. 

Then add the variables in the `/templates/roles/routers/vars/main.yml` 

Ensure your inventory hostnames match the hostnames in the vars file 

Any questions just email roger at rogerperkin.co.uk or visit 
https://www.rogerperkin.co.uk and send me a message 

Enjoy! 

Roger 
CCIE #50038 

