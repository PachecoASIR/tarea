ping: apt-get update && apt-get install -y iputils-ping
traceroute: apt-get install traceroute
mtr: apt-get install mtr
ifconfig: apt-get install net-tools
ifup/ifdown: apt-get install ifupdown
ip address: ip address show (ya estaba instalado)
host: apt-get install host
route: route -n (venía preinstalado)
ifplugstatus: apt-get install ifplugd
netstat: netstat (venía preinstalado)
whois: apt-get install whois
curl: apt-get install curl
dig: apt-get install dnsutils
Para editar resolv.conf para que el DNS cliente sea otro contenedor:
nano /etc/resolv.conf
Modificamos el nameserver con la IP del otro contenedor.
Una vez hecho esto al hacer un dig la IP de SERVER ha de ser igual a IP de contenedor.