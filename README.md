# FreeBSD-NewWireGuard-Config
Facilitador de criação de chaves e confgiuração para WireGuard em FreeBSD

Para usar o script as variáveis serveraddress lanadddress e vpnaddres devem ser definidas como no seguinte exemplo

set serveraddress = mywgserver.domain.tld

set lanaddress = 192.168.0.0/24

set vpnaddress = 10.0.0.0/24


O arquivo /usr/local/etc/wireguad/wg0.conf de exemplo é:

[interface]
 PrivateKey = wg0.key
 ListenPort = 51820
 Address = 10.0.0.1/24

