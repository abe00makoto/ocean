ocean
=====

DegitalOcean WebApi commandline wrapper

[DegitalOcean is Simple Cloud Hosting for Developpers]((https://www.digitalocean.com/?refcode=58b04120b7b2)



##INSTALL

```
wget https://raw.github.com/abe00makoto/ocean/master/ocean
chmod +x ocean

vim ~/.bash_profile

export OCEAN_API_KEY=xxxxxxxx
export OCEAN_CLIENT_ID=xxxxxxxx

```

##Run

ex) server restart
```
ocean droplets server01 reboot
```
ex) server make

```
ocean droplets new droplet_name=abe05 size_id=512MB image_id='CentOS 6.4 x32' region_id='Amsterdam 1' ssh_key_id1=abe00makoto
```
ex) if miss typed.

```
ocean droplets new droplet_name=abe05 size_id=512MB image_id='CentOS 6.4 x32' region_id=??? ssh_key_id1=abe00makoto

name resolution error:region_id:[???]
please select from
[Amsterdam 1] 
[San Francisco 1] 
[New York 2] 


```

```
usage:
	ocean droplets
	ocean droplets new droplet_name=<droplet_name> size_id=<size_id> image_id=<image_id> region_id=<region_id>
	ocean droplets new droplet_name=<droplet_name> size_id=<size_id> image_id=<image_id> region_id=<region_id> ssh_key_id1=<ssh_key_id1>
	ocean droplets new droplet_name=<droplet_name> size_id=<size_id> image_id=<image_id> region_id=<region_id> ssh_key_id1=<ssh_key_id1> ssh_key_id2=<ssh_key_id2>
	ocean droplets <droplet_id>
	ocean droplets <droplet_id> reboot
	ocean droplets <droplet_id> power_cycle
	ocean droplets <droplet_id> shutdown
	ocean droplets <droplet_id> power_off
	ocean droplets <droplet_id> power_on
	ocean droplets <droplet_id> password_reset
	ocean droplets <droplet_id> resize size_id=<size_id>
	ocean droplets <droplet_id> snapshot snapshot_name=<snapshot_name>
	ocean droplets <droplet_id> restore image_id=<image_id>
	ocean droplets <droplet_id> rebuild image_id=<image_id>
	ocean droplets <droplet_id> enable_backups
	ocean droplets <droplet_id> disable_backups
	ocean droplets <droplet_id> rename name=<name>
	ocean droplets <droplet_id> destroy
	ocean regions
	ocean images
	ocean images <image_id>
	ocean images <image_id> transfer region_id=<region_id>
	ocean ssh_keys
	ocean ssh_keys new ssh_key_name=<ssh_key_name> ssh_public_key=<ssh_public_key>
	ocean ssh_keys <ssh_key_id>
	ocean ssh_keys <ssh_key_id> edit
	ocean ssh_keys <ssh_key_id> destroy
	ocean sizes
	ocean domains
	ocean domains new domain=<domain> ip_address=<ip_address>
	ocean domains <domain_id>
	ocean domains <domain_id> destroy
	ocean domains <domain_id> records
	ocean domains <domain_id> records new record_type=<record_type> data=<data>
	ocean domains <domain_id> records <record_id>
	ocean domains <domain_id> records <record_id> edit
	ocean domains <domain_id> records <record_id> destroy
```

	
	
	

