ansible-playbook for setup zabbix-server and zabbix-proxy

*Requirements*
docker >=18.09
docker-compose >=1.21.0
ansible >=2.8.6

1. Run zabbix-server and zabbix-proxy on the same host:
	ansible-playbook main.yml

2. Run installation only zabbix-server:
	ansible-playbook main.yml --tags "zabbix-server"

3. Run installation only zabbix-proxy:
	ansible-playbook main.yml --tags "zabbix-proxy"

You must enter password for postgres, IP address for ICMP monitoring (example 8.8.8.8) and the external address of the machine on which you install zabbix.
